# JS属性操作

## 属性

1. 属性就是人类对于一个物体**抽象方面的刻画**。

## JS中两种操作属性的方法

1. 点&rArr;**.**
   1. 元素.属性
2. 方括号&rArr;[ ]
   1. 元素['属性']

**方括号中可以填入需要计算的东西，或者不符合标识符规范的！**

## JS读与写的操作

```Javascript
ele.style.background;//读
ele.style.background = 'red';//写
```

## 常用属性

1. id

2. className

3. value

   ```html
   <input id="input1" type="text" value="请输入密码">
   <script> 
      var input1 = document.getElementById('input1');
      console.log(input1.value);
   </script>
   ```

4. style
   1. background

   2. color

   3. width

   4. height

   5. cssText

      ```html
      <div id="box" class="active"></div>
      <script> 
      var box = document.getElementById('box');
      box.onclick = function(){
      	box.style.cssText = 'width:300px;height:300px;background:green;'
      }
      </script>
      ```

5. innerHTML

   ```html
   <p id="txt">
      这是文字内容121212
      <span>这是副标题</span>
   </p>
   <script> 
   var txt = document.getElementById('txt');
   txt.innerHTML = '123456';
   </script>
   ```

6. href

   ```html
   <style>
       a{
        font-size: 20px;
       }
       img{
        display: block;
        width: 400px;
       }
   </style>
   <a id="link" href="1.属性操作一.html">链接</a>
   <script> 
   	var link = document.getElementById('link');
   	console.log(link.href);
   </script>
   ```

7. src

   ```html
    <img id="img" src="img\a.jpg" alt="">
   <script>
       var img = document.getElementById('img');
       console.log(img.src);
   </script>
   ```

8. tagName

   ```html
   <a id="link" href="1.属性操作一.html">链接</a>
   <img id="img" src="img\a.jpg" alt="">
   <script>
       var link = document.getElementById('link');
       var img = document.getElementById('img');
   
       console.log(link.tagName);
       console.log(img.tagName);
   </script>
   ```

## 属性操作时的注意事项及常见问题

1. href和src值获取到的是绝对路径
2. style是间隔属性
3. cssText会替换掉当前所有的行间隔
4. class是关键字，改成className
5. tagName获取到的是大写字母