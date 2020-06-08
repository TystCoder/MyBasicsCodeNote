## write
命令名称：
* write
 
命令所在路径：
* /usr/bin/write

执行权限：
* 所有用户

语法：
* write<用户名>

功能描述：
* 给用户发信息，以Ctrl+D保存结束

范例：
* write linzhiling

----
## wall
命令名称：
* wall

命令英文原意：
* **wr**ite **all**
 
命令所在路径：
* /usr/bin/wall

执行权限：
* 所有用户

语法：
* wall [message]

功能描述：
* 发广播信息

范例：
* wall ShenCHao is a honest man!

----
## ping
命令名称：
* ping
 
命令所在路径：
* /bin/ping

执行权限：
* 所有用户

语法：
* ping 选项 IP地址
    * -c 指定发送次数 

功能描述：
* 测试网络连通性

范例：
* ping 192.168.109.0

----
## ifconfig
命令名称：
* ifconfig

命令英文原意：
* **i**nter**f**ace **config**ure
 
命令所在路径：
* /sbin/ifconfig

执行权限：
* root

语法：
* ifconfig 网卡名 IP地址

功能描述：
* 查看和设置网卡信息

范例：
* ifconfig eth0 192.168.109.0

----
## mail
命令名称：
* mail
 
命令所在路径：
* /bin/mail

执行权限：
* 所有用户

语法：
* mail[用户名]

功能描述：
* 查看发送电子邮件

范例：
* mail root

----
## last
命令名称：
* last
 
命令所在路径：
* /usr/bin/last

执行权限：
* 所有用户

语法：
* last

功能描述：
* 列出目前与过去登入系统的用户信息

范例：
* last

----
## lastlog
命令名称：
* lastlog
 
命令所在路径：
* /usr/bin/lastlog

执行权限：
* 所有用户

语法：
* lastlog

功能描述：
* 检查某特定用户上次登录时间

范例：
* lastlog
* lastlog -u 502

----
## traceroute
命令名称：
* traceroute
  
命令所在路径：
* /bin/traceroute

执行权限：
* 所有用户

语法：
* traceroute

功能描述：
* 显示数据包到主机间的路径

范例：
* traceroute www.sina.com.cn

----
## netstat
命令名称：
* netstat

命令英文原意：
* /bin/netstat
 
命令所在路径：
* 所有用户

执行权限：
* 所有用户

语法：
* netstat [选项]

选项
* -t:TCP协议
* -u:UDP协议
* -l:监听
* -r:路由
* -n:显示IP地址和端口号

功能描述：
* 显示网络相关信息

范例：
* netstat -tlun  查看本机监听的端口
* netstat -an 查看本机所有的网络连接
* netstat -rn 查看本机路由表

----
## setup
命令名称：
* setup
 
命令所在路径：
* /usr/bin/setup

执行权限：
* root

语法：
* setup

功能描述：
* 配置网络

范例：
* setup

----
## 挂载命令
命令名称：
* mount
 
命令所在路径：
* /bin/mount

执行权限：
* 所有用户

语法：
* mount [-t 文件系统]设备文件名 挂载点

范例：
* mount -t iso9660 /dev/sr0 /mnt/cdrom

----