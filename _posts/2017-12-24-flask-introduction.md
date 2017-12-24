# Flask入门笔记
## 简介
Flask是Python编写的一个轻量级Web应用框架。

## 安装
安装过程十分简单，方式也很多，可以自由选择
官网安装：[http://docs.jinkan.org/docs/flask/installation.html#installation](http://docs.jinkan.org/docs/flask/installation.html#installation)

## 入门Demo
QuarkStart Demo

	from flask import Flask
	app = Flask(__name__)
	
	@app.route('/')
	def hello_world():
		return 'Hello World!'
	
	if __name__ == '__main__':
		app.run()

保存至hello.py，执行并访问http端口

> $ python hello.py
> Running on http://127.0.0.1:5000/

至此便启动了一个flask服务

## 配置
（1）调试模式

	app.debug = True 或 app.run(debug=True)
（2）路由

	@app.route('/hello', methods=[‘GET’,’POST’])
	def hello():
		return 'Hello World'
	动态URL参数
	@app.route('/user/<username>')
	def show_user_profile(username):
		return 'User %s' % username
（3）请求

	 from flask import request
	 # 获取表单数据
	 @app.route('/login', methods=['POST'])
	 def login():
		username = request.form['username']
		password = request.form['password']
		return ‘SUCCESS’
通过args属性来访问URL中提交的参数（?key=value）

	 searchword = request.args.get('q', '')

（4）日志记录
从Flask 0.3开始，Flask就已经预置了日志系统。

	app.logger.debug('A value for debugging')
	app.logger.warning('A warning occurred (%d apples)', 42)
	app.logger.error('An error occurred')
附带的 logger 是一个标准日志类 Logger ，所以更多信息请查阅[logging](https://docs.python.org/3/library/logging.html)

## 部署

## 参考
[快速入门](http://docs.jinkan.org/docs/flask/quickstart.html#quickstart)


