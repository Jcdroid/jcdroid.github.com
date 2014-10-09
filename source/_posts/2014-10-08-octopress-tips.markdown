---
layout: post
title: "Octopress Tips"
date: 2014-10-08 23:30:28 +0800
comments: true
published: true
categories: 
---
###目录
* [新窗口中打开超链接](#1)
* [添加Tag](#2)

####<a id="1"></a>新窗口中打开超链接
修改*_include\custom\head.html*如下即可

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

####<a id="2"></a>添加Tag
