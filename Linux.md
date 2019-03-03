
课程框架介绍：
	linux  操作系统  
	linux操作系统初识阶段
		linux认识以及基本命令操作
		linux常用工具（编辑器，调试器。。。。）
	linux系统编程阶段：
		进程概念---程序   ***^
		进程控制          **
		基础IO            **
		进程间通信        **
		进程信号          **
		多线程            ****
	linux网络编程阶段：
		网络基础1
		网络编程
		网络基础2
		网络基础3
		高级IO
        
基础命令
    ls -a workspace
    命令名称 [参数选项] [操作对象]
目录操作命令：
    ls  浏览目录，列出目录下的文件信息
        目录--文件夹
        -a  浏览所有文件，不忽略以.开头的文件
            查看隐藏文件
            linux下以.开头的文件默认是隐藏文件
            .   表示当前路径
            ..  当前路径的上一层路径
        -l  查看目录下文件的详细信息
            文件类型：- 普通文件  d 目录文件
    pwd 查看当前所在路径--
        -绝对路径：表示路径的时候，起始路径从根目录开始的路径
            在整个linux目录结构中一个文件的位置表示
        -相对路径：表示路径的时候，起始路径从当前路径开始的路径
            相对于当前所在路径，一个文件的位置表示
        linux目录结构：树形结构，根目录
    mkdir   创建目录
        -p  多层级递归创建目录，任意一层目录不存在都会被创建
    rmdir   删除空目录
        -p  多层级空目录的递归删除
    rm      默认删除普通文件
        -r  删除目录（递归删除目录下的所有文件）
        -f  忽略提示信息，直接进行操作
    cp      拷贝一个文件到指定路径下
        -r  拷贝目录（递归拷贝目录下的所有文件）
        -f  忽略提示信息，直接进行操作
    mv      移动一个文件到指定位置
        -i  增加提示信息
    cd      改变当前所在路径（进入指定目录）
        ~   快速回到当前用户的家目录
        -   快速返回上一次所在路径
普通文件操作命令：
    touch   刷新已存在的文件时间属性，若文件不存在则创建
        -d  以指定时间刷新属性 "2018-02-28 12:10:30"
        -r  以指定文件的时间属性刷新另一个文件
        -a  只刷新最后一次访问时间
        -m  只刷新最后一次修改时间
    cat     打印文件内容到显示终端
        -n  打印行号
    more    分页显示文件内容
        回车  向下按行滚动
        f     向下按页滚动
        b     向上按页滚动
        q     退出显示
    less    分页显示文件内容
        f     向下按页滚动
        b     向上按页滚动  
        j/k   上下按行滚动
        匹配查找字符串
        /string  向下匹配查找string字符串
        ?string  向上匹配查找string字符串
            n   继续查找下一个匹配位置
        q   退出显示
    head    默认显示文件前10行数据
        -n  指定显示文件前n行数据
    tail    默认显示文件末尾10行数据
        -n  指定显示文件末尾n行数据
        -f  持续刷新显示文件末尾新增数据
其它命令： 
    man 手册查看命令
    ifconfig    查看/设置网卡信息命令
    service network start 启动网络服务
    su  切换用户
        su root
    useradd  添加用户
        useradd -m zhang
    passwd   修改密码
        passwd zhang
    echo    打印字符串到终端显示
        echo "adsfd"
    |   管道符
        连接两个命令，将前边命令处理结果交给后边命令进行处理
    >>  重定向符
        改变数据流向，将要写入到终端显示的数据，写入到指定文件中
        echo "zhang" >> abc.txt
    
    
    
    
    
    
    
    
    