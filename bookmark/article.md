# 好文收藏
## HTML
* [Battling BEM – 5 common problems and how to avoid them](https://medium.com/fed-or-dead/battling-bem-5-common-problems-and-how-to-avoid-them-5bbd23dee319#.6jkw93axf)
	* 如嵌套太深 用新的组件

## CSS
* [浏览器的工作原理：新式网络浏览器幕后揭秘](http://www.html5rocks.com/zh/tutorials/internals/howbrowserswork/?from=timeline&isappinstalled=0)
* [12 Little-Known CSS Facts (The Sequel)](http://www.sitepoint.com/12-little-known-css-facts-the-sequel/) 介绍了一些CSS的你可能不知道的用法
* [是时候学习Postcss了](http://davidtheclark.com/its-time-for-everyone-to-learn-about-postcss/)
* [The CSS at…](https://css-tricks.com/css/) 一些大公司是怎么处理 CSS：预译器，前缀，代码风格等
* [2015 Codrops 一大波优秀的资源](http://tympanus.net/codrops2015/)
* [Blending Modes in CSS: Color Theory and Practical Application](http://webdesign.tutsplus.com/tutorials/blending-modes-in-css-color-theory-and-practical-application--cms-25201) 混合模式的不同值的颜色值算法。

### 酷炫效果
* [Star Wars 文字动画](https://cssanimation.rocks/starwars/)


## JS
### 介绍
* [A re-introduction to JavaScript (JS tutorial)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript)

### 代码质量
* [Superhero.js](http://superherojs.com/) 关于如何创建一个可维护的大型 JS 项目的一系列优秀文章
* [refactoring tales](http://javascriptplayground.com/the-refactoring-tales/refactoring-tales.html) 一些案例，应该如何重构
* [avoid forEach](http://aeflash.com/2014-11/avoid-foreach.html)

### 工具方法
* [7 Essential JavaScript Functions](https://davidwalsh.name/essential-javascript-functions)

## 技巧
* [The Art of Debugging(调试的艺术)](https://remysharp.com/2015/10/14/the-art-of-debugging)
	* 重现 Bug
	* 理解 Bug 是如何产生的
	* 解决 Bug
* [JS 做后台任务](http://www.sitepoint.com/how-to-schedule-background-tasks-in-javascript/)
用 requestIdleCallback。 这个方法会在浏览器空闲时做一些事情。用法，如
```
f ('requestIdleCallback' in window) {
  // requestIdleCallback supported
  requestIdleCallback(backgroundTask);
}
else {
  // no support - do something else
  setTimeout(backgroundTask1, 1);
  setTimeout(backgroundTask2, 1);
  setTimeout(backgroundTask3, 1);
}
```


## 其他
* [The state of Web Components](https://hacks.mozilla.org/2015/06/the-state-of-web-components)
* [10 Interview Questions Every JavaScript Developer Should Know](https://medium.com/javascript-scene/10-interview-questions-every-javascript-developer-should-know-6fa6bdf5ad95#.hbilswjcl)

