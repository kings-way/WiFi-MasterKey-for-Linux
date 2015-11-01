# WiFi-MasterKey-in-Linux
## WiFi 万能钥匙 for Linux
### Notice
* 本代码fork自 https://github.com/5alt/lianwifi
* 源代码模拟了OS X下Wifi万能钥匙的运行过程，也仅适用与OS X操作系统
* 于是我就简单修改了一下，使其适用于Linux环境

### Usage 

* 运行环境准备

		sudo apt-get install python-pip wireless-tools
		sudo pip install  requests pycrypto

* 直接运行即可自动搜索周围AP信号，随后自动调用wifi万能钥匙查询接口，返回有密码的条目
* 

		chmod +x test.py
		./test.py

### Ps：更多细节功能尽请期待！
