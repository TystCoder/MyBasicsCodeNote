## locate
命令名称：
* locate

命令所在路径：
* /usr/bin/locate

执行权限：
* 所有用户

语法：
* locate 文件名

功能描述：
* 在文件资料库中查找文件

范例：
* locate inittab
----
## which
命令名称：
* which
 
命令所在路径：
* /usr/bin/which

执行权限：
* 所有用户

语法：
* which 命令

功能描述：
* 搜索命令所在目录及别名信息

范例：
* which ls

----
## whereis
命令名称：
* whereis
 
命令所在路径：
* /usr/bin/whereis

执行权限：
* 所有用户

语法：
* whereis [命令名称]

功能描述：
* 搜索命令所在目录及帮助文档路径

范例：
* whereis ls

----
## grep
命令名称：
* grep
 
命令所在路径：
* /bin/grep

执行权限：
* 所有用户

语法：
* grep -iv [指定字符串] [文件]

功能描述：
* 在文件中搜寻字符串匹配的行并输出
* -i 不区分大小写
* -v 排除指定字符串

范例：
* grep mysql /root/install.log

----