# R install

* 下载R源代码

 [原码下载地址](https://cloud.r-project.org/)
  
* 安装编译环境

    yum -y install gcc
    
    yum install glibc-headers
    
    yum install gcc-c++
    
    yum install gcc-gfortran

* 安装

    在下载的解压文件夹中 
    ./configure 
    
    make 
    
    make install
    
安装过程中的问题

* 1、问题描述：checking whether zlib support suffices… configure: error: zlib library and headers are required  

      解决方法：yum -y install bzip2-devel 

* 2、问题描述：configure: error: “liblzma library and headers are required” 

        解决方法：yum -y install xz-devel.x86_64 

* 3、缺少什么就使用yum search 缺少的名称，再根据相应的包来进行安装。

* 4、yum install readline-devel（解决错误“ --with-readline=yes (default) and headers/libs are not available”）

* 5、yum install libXt-devel（解决错误“–with-x=yes (default) and X11 headers/libs are not available”）
