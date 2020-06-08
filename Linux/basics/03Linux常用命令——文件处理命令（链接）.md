# 文件处理命令：ln
1. 命令名称：ln
2. 命令英语原意：__l__ i __n__ k
3. 命令所在路径：/bin/ln
4. 执行权限：所有用户
5. 语法：
    * ln -s [原文件] [目标文件]
        * -s 创建软连接
6. 功能描述：生成链接文件
7. 范例：
    * ln -s /etc/issue&nbsp;&nbsp;/tmp/issue.soft
        * 创建文件/etc/issue的软连接/tmp/issue.soft
    * ln /etc/issue&nbsp;&nbsp;/tmp/issue.hard
        * 创建文件/etc/issue的硬链接/tmp/issue.hard
# 软连接特征：类似Windows快捷方式
1. lrwxrwxrwx __l软连接__
    * 软件权限：rwxrwxrwx
2. 文件大小-只是符号链接
3. /tmp/issue.soft->/etc/issue
    * 箭头指向源文件
# 硬链接特征：
1. 拷贝cp -p + 同步更新
    * echo "www.aljdl.net">>/etc/issue
2. 通过i节点识别
3. 不能跨分区
4. 不能针对目录使用