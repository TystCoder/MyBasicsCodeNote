## 什么是for循环

for循环用来重复不断的做一件事

## for循环语法

```javascript
for(初始值;循环条件;自增条件){
	//执行条件
}
```

模拟多选

```html
<div class="box">
      <h3>模拟复选</h3>
      <div class="option">
        <a href="javascript:;">美食</a>
        <a href="javascript:;">逛街</a>
        <a href="javascript:;">旅游</a>
      </div>
    </div>
    <script>
     //获取一组a标签
     var btns = document.querySelectorAll('.option a');
   
     //for 给一组元素加事件
     for(var i = 0;i<btns.length;i++){
		 //自定义属性
		 btns[i].abc=false;
		 
     	btns[i].onclick=function(){
			
			//在事件函数内不能之间使用i
			//添加条件判断
			if(this.abc==true){
				this.className='';
			}else{
				this.className='checked';
			}
			
			//取反
			this.abc=!this.abc;
			
			//第一版
     		// 操作对于按钮class
     		// this.className='checked';
     	}
     }

    </script>
```

模拟单选

```html
<link rel="stylesheet" href="./radio.css">
  </head>
  <body>
    <div class="box">
      <div class="option">
        <a href="javascript:;">男</a>
        <a href="javascript:;">女</a>
        <a href="javascript:;">保密</a>
      </div>
    </div>
    <script>
		var btns = document.querySelectorAll('.option a');
		//1.for 添加点击事件
		for(var i=0;i<btns.length;i++){
			
			btns[i].onclick=function(){
				//需要操作一组元素的时候，就要想到for
				
				//2.点击某一个按钮之后，先将 所有按钮class都变空
				for(var j=0;j<btns.length;j++){
					btns[j].className='';
				}
				
				//3.在找到对应点击的那个按钮，给他单独加上 clas checked
				this.className='checked';
			}
		}
    </script>
```

元素自定义

```html
<div class = "box" id = "abc"></div>
<script>
	var div = document.querySelectorAll('div')[0];
    //操作元素属性
    //div.title='开课吧';
    
    //自定义属性
    div.abc='哈哈哈';
    
    //自定义属性f12是看不到的，但是是可以获取的
    console.log(div.abc);
</script>
```

