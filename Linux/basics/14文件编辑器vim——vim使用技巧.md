* 导入命令执行结果
    * :r 
    * !命令
* 定义快捷键:map 快捷键 出发命令
    * 范例：
        * :map ^P I#\<ESC\>
        * :map ^B 0x
* 连续行注释
    * :n1,n2s/^/#/g
    * :n1,n2s/^#//g
    * :n1,n2s/^/W/g
* 替换
    * :ab mymail samlee@lampbrother.net