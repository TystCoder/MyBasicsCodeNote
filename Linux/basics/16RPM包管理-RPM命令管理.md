# RPM包命令管理
## RPM包命名原则
* httpd-2.2.15-15.el6.centos.1.i686.rpm
    * httpd&nbsp;&nbsp;&nbsp;&rArr;&nbsp;软件包名
    * 2.2.15&nbsp;&rArr;&nbsp;软件版本
    * 15&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&rArr;&nbsp;软件发布的次数
    * el6.centos&rArr;适合的Linux平台
    * i686&nbsp;&nbsp;&nbsp;&nbsp;&rArr;&nbsp;适合的硬件平台
    * rpm&nbsp;&nbsp;&nbsp;&nbsp;&rArr;&nbsp;rpm包扩展名 
## RPM包依赖性
* 树形依赖
    * a&rArr;b&rArr;c
* 环形依赖
    * a&rArr;b&rArr;c&rArr;a
* 模块依赖
    * 模块依赖查询网站
        * www.rpmfind.net
## 包全名与包名
* 包全名
    * 操作的包是没有安装的软件包时，使用包全名。而且需要注意路径
* 包名
    * 操作已经安装的软件包时，使用包名。是搜索/var/lib/rpm/中的数据库
## RPM安装
* rpm -ivh 包全名
    * -i（install）&rArr;&nbsp;安装
    * -v（verbose）&rArr;&nbsp;显示详细信息
    * -h（hash）&rArr;&nbsp;显示进度
    * --nodeps&nbsp;&rArr;&nbsp;不检测依赖性
## RPM包升级
* rpm -Uvh 包全名
    * -U（upgrade）&rArr;升级
## 卸载
* rpm -e 全名
    * -e（erase）&nbsp;&rArr;&nbsp;卸载
    * --nodeps &nbsp;&rArr;&nbsp;不检查依赖性
## 查询是否安装
* rpm -q 包名
    * -q（query）&rArr;&nbsp;查询
* rpm -a
    * -a（all）&rArr;&nbsp;所有
## 查询软件包详细信息
* rpm -qi 包名
    * -i（information）&rArr;&nbsp;查询软件信息
    * -p（package）&rArr;&nbsp;查询未安装包信息
## 查询包中文件安装位置
* rpm -ql 包名
    * -l（list）&rArr;&nbsp;列表
    * -p（package）&rArr;&nbsp;查询未安装包信息
## 查询系统文件属于哪个RPM包
* rpm -qf 系统文件名
    * -f（file）&rArr;&nbsp;查询系统文件属于哪个软件包
## 查询软件包的依赖性
* rpm -qR 包名
    * -R（requires）&rArr;&nbsp;查询软件包的依赖性
    * -p（package）&rArr;&nbsp;查询未安装包信息

