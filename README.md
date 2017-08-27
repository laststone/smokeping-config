# smokeping-config
CentOS6.5中：smokeping安装与配置项



推荐安装资料：http://blog.csdn.net/fairplay_li/article/details/45817095
推荐配置资料：http://www.xuliangwei.com/xubusi/507.html?utm_source=tuicool&utm_medium=referral


首先，安装阿里源
接着，按照安装资料进行安装
	三个安装包rz上来解压安装即可
	安装echoping注意：执行 yum install -y popt*
	                  ./configure 加上--without-libidn选项
然后，httpd的配置使用给定的配置文件覆盖即可
之后，smokeping的配置复制使用给定的配置文件即可
最后，按照配置资料进行配置，设置service管理和开机自启
（注意：全程关闭iptables和selinux）