---
layout: post
title: Hello world!
category: reading
---


Fork from http://darktea.github.io/

现在，我可以：

* 使用纯文本的[Markdown]编辑文章
* 使用git维护文章的版本
* 不用租一个虚拟空间和数据库服务，而就在[GitHub]上托管整个网站
* 自定义域名指向
* 使用[Disqus]的云评论服务
* 一如既往的使用[Google Picasa]作为我的图片外链服务
* 用[Google Custom Search]自定义站内搜索
* [jekyll]自带的或者用[HighlightJS]做代码高亮
* [Gravatar]统一头像标识服务
* ……

# a
>a
 b
[baidu](http://www.baidu.com)

*莫愁前路无知己，[**天下**]谁人不识君*

* 一盏灯

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

dog | bird | cat
----|------|----
foo | foo  | foo
bar | bar  | bar
baz | baz  | baz

*   This is a list item with two paragraphs.

    This is the second paragraph in the list item. You're
only required to indent the first line. Lorem ipsum dolor
sit amet, consectetuer adipiscing elit.

*   Another item in the same list.

*   A list item with a blockquote:

    > This is a blockquote
    > inside a list item.

Here is an example of AppleScript:

    @RequestMapping(value = "/similarity/search", method = RequestMethod.POST)
    @ResponseBody
    public APIResult similaritySearch(@RequestBody PoiBaseModel searchParam) {
        try {
            return apiDataService.similaritySearch(searchParam);
        }catch(ServiceException se){
            LOG.error("invoke similaritySearch occur ServiceException ",se);
            return APIUtils.getResponse(se);
        }catch(Exception e){
            LOG.error("invoke similaritySearch occur Exception",e);
            return APIUtils.getResponse(e);
        }
    }
    
    
 <meueax@gmail.com>


![][1]
[1]: http://latex.codecogs.com/gif.latex?\prod%20\(n_{i}\)+1

![](http://ww4.sinaimg.cn/bmiddle/aa397b7fjw1dzplsgpdw5j.jpg)



感谢这个有云的时代！可以让我们通过一件件简单的工具打造属于每个程序员自己的站点，[像黑客一样写博客](http://kyle.xlau.org/posts/blogging-like-a-hacker.html)（原文：[Blogging Like a Hacker](http://tom.preston-werner.com/2008/11/17/blogging-like-a-hacker.html)）。

{% include references.md %}
