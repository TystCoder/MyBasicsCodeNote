#  querySelector获取元素

## document.querySelector()

```javascript
document.querySelector('元素选择器');
```

* 获取元素，通过元素选择器来选择

## 特性

1. 通过选择器进行获取
2. 遇到第一个符合条件的元素，就返回第一个元素
3. 如果获取一个不存在的元素，得到的结果是null！！！
4. document/parent.querySelector('选择器');
5. IE8以下不可以使用！！！

```html
<section class="warp">
	<div>盒子</div>
</section>
<script>
	//在父级下找到某个元素
    console.log(document.querySelector('.warp').querySelector('div'))
</script>
```

