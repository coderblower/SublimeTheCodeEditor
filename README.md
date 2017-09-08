# Sublime text snippet 
## For wordpress -> sytle.css ( tab trigger " `theme_info`")


```
//Input:

<snippet>
	<content><![CDATA[
/*
Theme Name: ${1:Avira}
Theme URI: ${2:https://wordpress.org/themes/}
Author: ${3:We-love-coding}
Author-URI: ${4:https: https://wordpress.org/}
Description: ${5:Avera is an alignet theme for }
Version: ${6:1.3}
License: ${7:GNU General Public License v2 or later}
License URI: ${8:http://www.gnu.org/licenses/gpl-2.0.html}
Tags: ${9:one-column,two-columns, right-sidebar, accessibility-ready, custom-background, custom-colors, custom-header, custom-menu, editor-style, featured-images, flexible-header, microformats, post-formats, rtl-language-support, sticky-post, threaded-comments, translation-ready, blog} 
Text Domain: ${10:twentysixteen This theme, like WordPress, is licensed under the GPL.
Use it to make something cool, have fun, and share what you've learned with others.
}*/]]></content>
	<!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
	<tabTrigger>theme_info</tabTrigger>
	<!-- Optional: Set a scope to limit where the snippet will trigger -->
	<scope>source.css</scope>
</snippet>

// Output: 

/*
Theme Name: Avira
Theme URI: https://wordpress.org/themes/
Author: We-love-coding
Author-URI: https: https://wordpress.org/
Description: Avera is an alignet theme for 
Version: 1.3
License: GNU General Public License v2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html
Tags: one-column,two-columns, right-sidebar, accessibility-ready, custom-background, custom-colors, custom-header, custom-menu, editor-style, featured-images, flexible-header, microformats, post-formats, rtl-language-support, sticky-post, threaded-comments, translation-ready, blog 
Text Domain: twentysixteen This theme, like WordPress, is licensed under the GPL.
Use it to make something cool, have fun, and share what you've learned with others.
*/

```
# Snippet For PHP 
### Tab trigger "`ph`"
```
// Input:
<snippet>
	<content><![CDATA[
<?php $1 ${2:?>}
]]></content>
	<!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
    <tabTrigger>ph</tabTrigger> 
	<!-- Optional: Set a scope to limit where the snippet will trigger -->
	<scope>source.php</scope> 
</snippet>

// Output:
<?php ?>
```



