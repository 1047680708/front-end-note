# jQuery 选取元素概要
## 用选择器选取元素
```
$(选择器 [, 父元素])
```

支持选择器包括：
* CSS 1-3 定义的选择器。
* jQuery 自定义的选择器。

### 一些有用的选择器
* [:visible](https://api.jquery.com/visible-selector/) 可见元素
* [:hidden](https://api.jquery.com/hidden-selector/) 不可见元素
* [:animated](https://api.jquery.com/animated-selector/) 正在做动画的元素
* [:checked](https://api.jquery.com/checked-selector/) 选中的单选和复选按钮
* [:selected](https://api.jquery.com/selected-selector) 选中的 `<option>` 元素
* [:disabled](https://api.jquery.com/disabled-selector) 不可用的表单元素
* [:contains(文本)](https://api.jquery.com/contains-selector) 如： `$("div:contains('John')")`
* [:empty](https://api.jquery.com/empty-selector/) 没有子元素或没有文本内容的元素
* [:has(选择器)](https://api.jquery.com/has-selector/) 有指定子元素的元素

### 选择器中包含元字符的处理
选择器的元字符有：`!"#$%&'()*+,./:;<=>?@[\]^{|}~`。

选择器中如果要使用选择器的元字符，必须用`\\`来转义。如选择 id 为 `id="foo.bar"` 元素，要使用`$("#foo\\.bar")`。

## 从层级中选取元素
### 从父元素和祖系元素中找
* [.closest([选择器])](https://api.jquery.com/closest)
* [.parent([选择器])](https://api.jquery.com/parent)
* [.parents([选择器])](https://api.jquery.com/parents)
* [.offsetParent()](https://api.jquery.com/offsetParent) 找最近的父级定位元素（position 不为 static 的元素）

### 从子元素中下找
* [.find([选择器])](https://api.jquery.com/find/)
* [.children([选择器])](https://api.jquery.com/children/)
* [.contents()](https://api.jquery.com/contents/) 元素下的内容：包括文本节点和注释节点。常常也用来做选取 iframe 的内容，如
```
$('#frameDemo').contents().find('a');
// 等效与
$('#frameDemo')[0].contentWindow.$('a');

```

### 从兄弟元素中找
* [.siblings(选择器)](https://api.jquery.com/siblings/)
* [.prev()](https://api.jquery.com/prev)
* [.prevAll()](https://api.jquery.com/prevAll)
* [.next()](https://api.jquery.com/next)
* [.nextAll()](https://api.jquery.com/nextAll)


## 过滤掉不满足条件的元素
* [.filter(选择器|函数)](https://api.jquery.com/filter) 如:
```
$(".btn")
  .filter(function(index) {
    return index > 2 && $(this).is(':visible');
});
```

