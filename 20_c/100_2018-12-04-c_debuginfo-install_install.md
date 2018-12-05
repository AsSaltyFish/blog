Centos 7 系统，使用gdb调试C程序时，运行命令*r*un时出现如下错误：  
> Missing separate debuginfos, use: debuginfo-install glibc-2.17-222.el7.x86_64

解决方法：  
第一步： 安装debuginfo-install  

     yum install -y yum-utils

第二步：安装glibc-2.17  

     debuginfo-install -y glibc-2.17

总结：debuginfo-install 命令包含于yum-utils 中。
