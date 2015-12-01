# 字体
选择合适的字体，对提高网页的美观度和可读性有着举足轻重的作用。


## 字体基础知识
* [web安全字体](http://web.mit.edu/jmorzins/www/fonts.html)
* 字体栈(font-family)
	* [cssfontstack](http://www.cssfontstack.com/) 各种字体在系统的安装比例
	* [Font Stacks snippet](http://css-tricks.com/snippets/css/font-stacks/)

## 优化
### [使Chrome字体渲染更平滑](http://swordair.com/smoother-font-randering-in-chrome/)
Chrome在字体大于48px时，锯齿很明显。     
解决
普通文字用
```
text-rendering: optimizeLegibility;
-webkit-font-smoothing: antialiased;
```

icon font用用SVG替代WOFF。    
例如
```
@font-face {
  font-family: 'FontAwesome';
  src: url('../fonts/fontawesome-webfont.eot?v=4.1.0');
  src: url('../fonts/fontawesome-webfont.eot?#iefix&v=4.1.0') format('embedded-opentype'), url('../fonts/fontawesome-webfont.woff?v=4.1.0') format('woff'), url('../fonts/fontawesome-webfont.ttf?v=4.1.0') format('truetype'), url('../fonts/fontawesome-webfont.svg?v=4.1.0#fontawesomeregular') format('svg');
  font-weight: normal;
  font-style: normal;
}

@media screen and (-webkit-min-device-pixel-ratio:0) { /* 对chrome */
    @font-face {
        font-family: 'FontAwesome';
        src: url('../fonts/fontawesome-webfont.svg?v=4.1.0#fontawesomeregular') format('svg');
    }
}
```
注：更新到了chrome37，chrome字体渲染问题居然已经被解决了。

### [10个增强WEB字体排版的JQUERY插件](http://www.uisdc.com/10-jquery-plugins-to-enhance-your-web-typography)