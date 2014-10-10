---
layout: post
title: "Octopress Tips"
date: 2013-10-08 23:30:28 +0800
comments: true
published: true
categories: Octopress

---
&nbsp;

###目录
* [新窗口中打开超链接](#新窗口中打开超链接)
* [添加Categories](#添加Categories)
* [添加继续阅读](#添加继续阅读)
* [文章显示数量设定](#文章显示数量设定)
* [参考](#参考)

<!--more-->

####<a id="新窗口中打开超链接"></a>新窗口中打开超链接
修改`_include\custom\head.html`如下即可

```js
<script type="text/javascript">
	function addBlankTargetForLinks () {
  		$('a[href^="http"]').each(function(){
			$(this).attr('target', '_blank');
		});
	}
 
	$(document).bind('DOMNodeInserted', function(event) {
		addBlankTargetForLinks();
	});
</script>
```

参考：`https://gist.github.com/azone/4523641`

####<a id="添加Categories"></a>添加Categories


####<a id="添加继续阅读"></a>添加继续阅读


####<a id="文章显示数量设定"></a>文章显示数量设定


####<a id="参考"></a>参考
* [Octopress文章摘要显示和主页显示文章数量设定](http://blog.csdn.net/hankai1024/article/details/12850413)
