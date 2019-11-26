搭建环境须知.md

##在linux下搭建环境

###step1 安装python3.6
	
	$add-apt-repository ppa:jonathonf/python-3.6
	$apt-get update
	$apt-get install python3.6

###step2 更改python3软链接
	
	$rm -rf /usr/bin/python3
	$ln -s /usr/bin/python3.6 /usr/bin/python3

###step3 安装pip3
	
	$apt-get install python3-pip
使用pip3 -V查看pip3版本，如不是python3.6则升级
	
	$curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
	$python3.6 get-pip.py --force-reinstall


###安装其他依赖包
	
	$apt-get install libpython3.6-dev
	$pip3 install numpy
	$pip3 install django==2.1.*
	$pip3 install channels
