# ECMAScript流程控制

## 分支结构

### if

```javascript
//单条件判断
if(条件){}
if(条件){
    
}else{
    
}
//多条件
if(条件1){
    
}else if(条件2){
    
}
```

### switch

```javascript
switch(表达式||变量){
    case value1:
        console.log('执行的代码1');
        break;
    case value2:
        console.log('执行的代码2');
        break;
    case value3:
        console.log('执行的代码3');
        break;
    default:
        console.log('执行的代码4');
        break;
}
```

- switch后面的小括号内可以变量||表达式，一般都是变量
- value是与括号里的内容比较的，这个比较是全等的比较。
- 一旦满足全等的条件，就会执行后续的代码。
- default，以上条件都不满足的时候，执行这里对应的代码。
- default可以放在任何位置。

穿透

- 一旦符合条件，并且没有break终止后续代码，会产生穿透问题，当前满足条件的位置开始，后续的执行代码都会被执行。

**break**

- break后面的代码会终止执行，并跳出。

**所有的switch语句都可以用if语句替代**

### for

```javascript
for(初识化;循环条件;变更条件){

}
```

### for...in循环

```javascript
for(var key in obj){
	//这里的key指的就是对象下的属性
}
//例：
var obj = {
	x:20,
    y:30,
    z:40
}
for (var v in obj){
    //console.log(v);
    console.log(obj[v]);
}
var arr = [10,20,40,30];
for(var v in arr){
    console.log(arr[v]);
}
```

### while（前测试循环语句）

```javascript
while(判断条件){

}
```

### do while（后测试循环语句）

```javascript
do{
	//需要循环执行的代码
}while{
	//判断条件
}
```

**continue**

- 终止当前循环，包括continue后面的代码也会被终止执行，但是不跳出循环，循环会在这次之后，继续执行。