ccnt
====

校园网认证客户端，适用于武汉大学的神州数码认证

中国大陆地区校园网认证大多数是基于eap协议修改后
的私有协议，本程序仅仅实现了神州数码的认证过程，
但是可以方便地扩展。本程序使用C++，依赖libpcap库
（Windows中是Winpcap）,可在Linux与Windows中运行。

注意：本程序已在上述环境中测试通过，可以使用联网，
但是本程序不是一个完整的软件，仅仅是为了研究校园
网认证机制，若需要正常使用，请自行修改。

使用：
--- Linux ---
	(1) 安装libpcap相应的库
	(2) 在项目目录下执行 make

--- Windows ---
	(1) 需要首先安装WinPcap。www.winpcap.org
	(2) 将项目作为CodeBlocks工程打开，编译执行
	(3) 项目中用到C++11的一些特性，需要较高版本
		的编译器支持
	(4) 也可以直接编译，但要注意Codeblocks项目
		描述文件中的依赖关系与宏定义。
