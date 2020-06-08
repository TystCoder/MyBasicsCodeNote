# ECMAScript数据类型及类型转换

## ECMAScript数据类型划分

- 简单类型：
  - number&rArr;数字型
  - string&rArr;字符串型
  - boolean&rArr;布尔值型
    - true
    - false
  - null&rArr;空值
  - undefined&rArr;未定义
  - symbol&rArr;es6新增 唯一值/匿名的值
- 复杂类型：object&rArr;对象型

## 传值和传址

### 传值

- 简单数据类型&rArr;传值操作

### 传址

- 复杂数类型&rArr;传址操作(传的就是堆内的存储地址)

- ```javascript
  var arr = [1,2,3,4];
  arr[3] = 4;
  console.log(arr);
  ```

- js常见的对象类型：
  - Array
  - Object
  - Element
  - Elements
  - Function

## typeof运算符

- 类型检测
  - number
  - string
  - boolean
  - function
  - undefined
  - symbol
  - object

  ```javascript
  var a = null;
  console.log(typeof a);//object
  var fn = function(){}
  console.log(typeof fn);//function
  ```

## 强制数据类型转换

- 强制转换为数字
  - parselnt()

    - 转整数
    - 从左往右依次进行转换，当遇到非数字字符串时，停止转换，把后面的字符扔掉（只保留前面的！）
    - 如果首位字符是非数字字符，就转换成NaN(Not a  Number)&rArr;转换失败！

  - parseFloat()

    - 转浮点数
    - 从左往右依次进行转换，当遇到非数字字符串时，停止转换，把后面的字符扔掉（只保留前面的！）
    - 如果首位字符是非数字字符，就转换成NaN(Not a  Number)&rArr;转换失败！

  - Number()方法（推荐）
    
    - 转数字
    
    - 只要字符串内含有非数字字符串，就转成NaN
    
    - 只能转纯数字的字符串
    
      - 字符串转number规则
    
      - 布尔值转number规则
    
        - false&rArr;0
        - true&rArr;1
    
      - 对象转number规则
    
        - 通过js内部方法toString转换为字符串在通过Number()转换为数字
    
        - ```javascript
          var arr=[1,2,3];//NaN
          var arr=[10]
          //js内部方法toString();	
          //arr转换成字符串
          console.log(arr.toString());
          console.log(Number(arr));
          ```
    
      - null和undefined转换成number
    
  - isNaN和NaN

    - NaN&rArr;不是数字的数字，属于数据类型，但是不是一个具体的数；NaN谁都不等于，包括它自己
    - isNaN
      - 是一个方法，它可以用来判断数字是不是NaN
      - 当你不确定数值是否转换成功时，采用isNaN来判断
      - 结果返回布尔值

  - MAX_VALUE、MIN_VALUE、infinity

    - infinity&rArr;无穷大
    - -infinity&rArr;负无穷

- 强制转换为布尔值-Boolean()
  - 数字转换为布尔值规则
  - 字符串转换为布尔值规则
  - 对象转换为布尔值规则
  - null和undefined转换为布尔值规则

- 强制转换为字符串-String()
  - 数字、布尔值转换字符串规则
  - null和undefined转换为字符串规则
  - 对象转换字符串规则
    - 数组的toString
    - function的toString

- 运算符及隐式类型转换
  - 数学运算符的运算规则及相应的隐式类型转换规则
  - 赋值运算符的运算规则及相应的隐式类型转换规则
  - 比较运算符的运算规则及相应的隐式类型转换规则
  - 逻辑运算符的运算规则及相应的隐式类型转换规则
  - 三元运算符的运算规则



