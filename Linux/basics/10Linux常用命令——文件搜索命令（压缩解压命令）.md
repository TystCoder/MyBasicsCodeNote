## 压缩gzip
命令名称：
* gzip

命令英文原意：
* GUN zip
 
命令所在路径：
* /bin/gzip

执行权限：
* 所有用户

语法：
* gzip[文件]

功能描述：
* 压缩文件

压缩后文件格式：
* .gz

范例：
* 

----
## 解压gunzip
命令名称：
* gunzip

命令英文原意：
* GUN unzip
 
命令所在路径：
* /bin/gunzip

执行权限：
* 所有用户

语法：
* gunzip [压缩文件]

功能描述：
* 解压缩.gz的压缩文件

范例：
* gunzip boduo.gz

----
## 压缩解压tar
命令名称：
* tar
 
命令所在路径：
* /bin/tar

执行权限：
* 所有用户

语法：
* tar 选项[-zcf] [压缩后文件名] [目录]
    * -c 打包
    * -v 显示详细信息
    * -f 指定文件名
    * -z 打包同时压缩 

功能描述：
* 打包目录

tar命令解压缩语法：
* -x 解包
* -v 显示详细信息
* -f 指定压缩文件
* -z 解压缩

压缩后文件格式：

* .tar.gz

范例：
* tar -zxvf Japan.tar.gz

----
## 压缩zip
命令名称：
* zip
 
命令所在路径：
* /usr/bin/zip

执行权限：
* 所有用户

语法：
* zip 选项[-r] [压缩后文件名] [文件或目录]
* -r  压缩目录

功能描述：
* 压缩文件或目录

压缩后文件格式：
* .zip

范例：
* 

----
## 解压unzip
命令名称：
* unzip
 
命令所在路径：
* /usr/bin/unzip

执行权限：
* 所有用户

语法：
* unzip[压缩文件]

功能描述：
* 解压.zip的压缩文件

范例：
* unzip test.zip

----
## 压缩bzip2
命令名称：
* bzip2
 
命令所在路径：
* /usr/bin/bzip2

执行权限：
* 所有用户

语法：
* bzip2 选项[-k] [文件]
    * -k 产生压缩文件后保留原文件

功能描述：
* 压缩文件

压缩后文件格式：.bz2

范例：
* bzip2 -k boduo
* tar -cjf Japan.tar.bz2 Japan

----
## 解压bzip2
命令名称：
* bunzip2
 
命令所在路径：
* /usr/bin/bunzip2

执行权限：
* 所有用户

语法：
* bunzip2 选项[-k] [压缩文件]
    * -k 解压缩后保留原文件

功能描述：
* 解压缩

范例：
* bzip2 -k boduo.bz2
* tar -xjf Japan.tar.bz2