## find
命令名称：find
 
命令所在路径：
* /bin/find

执行权限：
* 所有用户

语法：
* find [搜索范围] [匹配条件]

功能描述：
* 文件搜索

范例：
* find /etc -name init
    * 在目录/etc中查找文件int
        * -iname 不区分大小写
* find / -size +204800
    * 在根目录下查找大于100MB的文件
        * +n——大于，-n——小于，n——等于
* find /home -user shenchao
    * 在根目录下查找所有者为shenchao的文件
        * -group 根据所属组查找
* find /etc -cmin -5
    * 在/etc下查找5分钟内被修改过属性的文件和目录
        * -amin——访问时间access
        * -cmin——文件属性change
        * -mmin——文件内容modify
* find /etc -size +163840 -a -size -204800
    * 在/etc下查找大于80MB小于100MB的文件
        * -a两个条件同时满足
        * -o两个条件满足任意一个即可
* find /etc -name inittab -exec ls -l {} \\;
    * 在/etc下查找inittab文件并显示其详细信息
        * -exec/-ok 命令 {} \\; 对搜索结果执行操作
* type 根据文件类型查找
    * f 文件
    * d 目录
    * l 软连接文件
* -inum 根据i节点查找
----