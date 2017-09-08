# License and package manager install

## sublime license
```
—– BEGIN LICENSE —–
Andrew Weber
Single User License
EA7E-855605
813A03DD 5E4AD9E6 6C0EEB94 BC99798F
942194A6 02396E98 E62C9979 4BB979FE
91424C9D A45400BF F6747D88 2FB88078
90F5CC94 1CDC92DC 8457107A F151657B
1D22E383 A997F016 42397640 33F41CFC
E1D0AE85 A0BBD039 0E9C8D55 E1B89D5D
5CDB7036 E56DE1C0 EFCC0840 650CD3A6
B98FC99C 8FAC73EE D2B95564 DF450523
—— END LICENSE ——
```

#Sublime 3 Package manager install

The simplest method of installation is through the Sublime Text console. The console is accessed via the `ctrl+`  shortcut or the` View > Show Console menu`. Once open, paste the appropriate Python code for your version of Sublime Text into the console

```
import urllib.request,os,hashlib; h = 'df21e130d211cfc94d9b0905775a7c0f' + '1e3d39e33b79698005270310898eea76'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```



#Sublime text User settings:

```{
	"color_scheme": "Packages/Agila Theme/Agila Dracula.tmTheme",
	"font_size": 12,
	"ignored_packages":
	[
		"Vintage"
	],
	"update_check": false,
 // ---------------------------  README -----------------------------------
    //  Copy these key/values to User/Preferences.sublime-settings
    //  They have NO effect here

    // If `true` will disable bindings like ctrl+alt+n etc
    // Handy for our italian friends :)
    "alt_gr": false,

    // If `true` will insert id="$1" snippet on pressing '#', similar on '.'
    // Useful for `raw html`, but annoying for some templating langs.
    "auto_id_class": false,

    // disable expanding abbreviation by Tab key
 // false value for disable snippet, And true for disable emmet pressing tab key. 
    "disable_tab_abbreviations": true,  

    // disable insertion of formatted linebreak when
    // Enter key is pressed between opening and closing HTML tags
    "disable_formatted_linebreak": false,

    // Enables default Emmet keymap. Many users complain that Emmet actions
    // (especially ones that bound to Alt key) behave incorrectly in 
    // non-English keyboard layouts. Set this setting to `false` in
    // Users’s Preferences.sublime-settings to disable all default
    // keybindings at once
    "enable_emmet_keymap": true,

    // disable expanding abbreviation by Tab key when autocomplete popup is visible
    "disable_tab_abbreviations_on_auto_complete": true

}
```


# Some Important Package to install 
`Emmet`
`Agila Theme` //  favorite color-scheme `Agila dracula`
`AdvanceNewFile`



# snippet For wordpress  sytle.css  tabtrigger " `theme_info`"


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



