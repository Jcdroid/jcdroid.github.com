---
layout: post
title: "Octopress Tips"
date: 2014-10-08 23:30:28 +0800
comments: true
categories: 
---
###目录
* 新窗口中打开超链接
* 添加Tag

####新窗口中打开超链接
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

####添加Tag
