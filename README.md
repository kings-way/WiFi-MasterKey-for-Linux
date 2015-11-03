# WiFi-MasterKey-for-Linux
## WiFi 万能钥匙 for Linux
### Notice:
* 本代码fork自 https://github.com/5alt/lianwifi
* 源代码模拟了OS X下Wifi万能钥匙的运行过程，也仅适用于OS X操作系统
* 于是我就简单修改了一下，使其适用于PC Linux以及Nokia N9手机

## Usage:
		$ chmod +x test.py
		$ ./test.py -h
		=====================
		Usage:
		   ./test.py    				run automaticly  
		   ./test.py  [ESSID] [BSSID]	query the specific ssid
		   ./test.py  -h				show this help notice
		=====================


## Preparation:

### for PC

		$ sudo apt-get install wireless-tools python-pip
		$ sudo pip install  requests pycrypto
		

### for Nokia N9
* N9自带python2.6, 我们还需要安装crypto和requests库，还要安装wireless-tools系统工具
* N9官方源早已失效，我用的第三方源中有python-crypto库和wireless-tools包，但是没有requests库，也没有python-pip工具，因此手动安装requests库
* 上述几个包都已经上传在For_Nokia_N9目录中，apt源不可用的同学可以下载下来，然后使用dpkg手动安装
 
		$ devel-su    //输入密码获得root权限
		# apt-get install wireless-tools python-crypto 
		# unzip requests-master.zip && cd requests-master
		# python setup.py install



### Ps：更多细节功能尽请期待！
