# JavaScript的位置

## 行间JS

```html
<div onclick="alter('我爱JavaScript')"></div>	
```

* 优势
  * 直接作用于当前元素
* 劣势
  * 复用率低
  * 结构不够清晰

## 内部JS

```html
<script>
//这里放置JS的代码	
</script>
```

* 优势
  * 代码分离清晰
  * 较利于后期修改维护
  * 同页面可以复用
* 劣势
  * 不同页面无法使用
  * 不同页面修改维护较麻烦

## 外部JS

```html
<script src="main.js"></scprit>
```

* 优势
  * 代码分离彻底
  * 利于后期维护修改
  * 不同页面之间也可以复用
* 缺点
  * 增强请求数量

