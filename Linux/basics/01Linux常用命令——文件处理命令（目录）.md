# 命令格式
1. 命令格式：命令 [-选项] [参数]
    * 例：ls -la /etc
2. 说明：
    * 1、个别命令使用不遵循此格式
    * 2、当有多个选项时，可以写在一起
    * 3、简化选项与完整选项
        * -a 等于 --all
# 目录处理命令：ls
1. 命令名称：ls
2. 命令英文原意：__l__ i __s__ t
3. 命令行所在路径：/bin/ls
4. 执行权限：所有用户
5. 功能描述：显示目录文件
6. 语法：ls 选项[-ald] [文件或目录]
    * -a（all） 显示所有文件，包括隐藏文件
    * -l（long） 详细信息显示
    * -d 查看目录属性
# -rw-r--r--
1. __-__ 文件类型（- 二进制文件 d目录 l软连接文件）
2. rw- r-- r--
    * rw- r-- r--
    * u   g   o
    * u所有者 g所属组 o其他人
    * r读    w写     x执行
# 目录处理命令：mkdir
1. 命令名称：mkdir
2. 命令英文原意：__m__ a __k__ e __dir__ ectories
3. 命令所在路径：/bin/mkdir
4. 执行权限：所有用户
5. 语法：mkdir -p [目录名]
6. 功能描述：创建新目录
    * -p 递归创建
7. 范例：
     * $mdkir -p /tmp/Japan/boduo
     * $mdkir -p /tmp/Japan/longze&nbsp;&nbsp;&nbsp;/tmp/Japan/cangjing
# 目录处理命令：cd
1. 命令名称：cd
2. 命令英语原意：__c__ hange __d__ irectory
3. 命令所在路径：shell内置命令
4. 执行权限：所有用户
5. 语法：cd [目录]
6. 功能描述：切换目录
7. 范例：
    * cd /tmp/Japanboduo 切换到指定目录
    * cd .. 回到上一级目录
# 目录处理命令：pwd
1. 命令名称：pwd
2. 命令英语原意：__p__ rint __w__ orking __d__ irectory
3. 命令所在路径：/bin/pwd
4. 执行权限：所有用户
5. 语法：pwd
6. 功能描述：显示当前目录
7. 范例：
    * pwd
        * /tmp/Japan/cangjing
# 目录处理命令：rmdir
1. 命令名称：rmdir
2. 命令英语原意：__r__ e __m__ ove empty __dir__ ectories
3. 命令所在路径：/bin/rmdir
4. 执行权限：所有用户
5. 语法：rmdir[目录名]
6. 功能描述：删除空目录
7. 范例：rmdir /tmp/Japan/boduo
# 目录处理命令：cp
1. 命令名称：cp
2. 命令英语原意：copy
3. 命令所在路径：/bin/cp
4. 执行权限：所有用户
5. 语法：cp -rp [原文件或目录] [目标目录]
    * -r 复制目录
    * -p 保留文件属性
6. 功能描述：复制文件或目录
7. 范例：
    * cp -r &nbsp;/tmp/Japan/cangjing &nbsp;/root
        * 将目录/tmp/Japan/cangjing复制到目录/root下
    * cp -rp &nbsp;/tmp/Japan/boduo &nbsp;/tmp/Japan/longze &nbsp;/root
        * 将/tmp/Japan目录下的boduo和longze目录复制到/root下，保持目录属性
# 目录处理命令：mv
1. 命令名称：mv
2. 命令英语原意：__m__ o __v__ e
3. 命令所在路径：/bin/mv
4. 执行权限：所有用户
5. 语法：mv [原文件或目录] [目标目录]
6. 功能描述：剪切文件、改名
# 目录处理命令：rm
1. 命令名称：rm
2. 命令英语原意：__r__ e __m__ ove
3. 命令所在路径：/bin/rm
4. 执行权限：所有用户
5. 语法：rm -rf [文件或目录]
    * -r 删除目录
    * -f 强制执行
6. 功能描述：删除文件
7. 范例：
    * rm /tmp/yum.log
        * 删除文件/tmp/yum.log
    * rm -rf /tmp/Japan/longze
        * 删除目录/tmp/Japan/longze
