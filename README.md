#
### 在diy-3.sh里面需要修改的东西
Diy_Core() {
	Author="281677160"       作者仓库
	Default_Device="x86-64"          机型名字，x86的就写x86-64的
	Updete_firmware="combined.img.gz"  安装使用的固件名字，一定要正确填写
	Extension=".img.gz"              安装使用固件的扩展（后缀），一定要正确填写
	Source="lede"               源码作者名字，随便写，用来区分源码的
}

#
---
- 机型名字可以看.config的第三行
CONFIG_TARGET_rockchip=y
CONFIG_TARGET_rockchip_armv8=y
CONFIG_TARGET_rockchip_armv8_DEVICE_friendlyarm_nanopi-r2s=y

- 上面的就是机型文件的三项，第三行的DEVICE_跟着的就是机型名字，后面的=y不要，就是friendlyarm_nanopi-r2s
- 就我知道没有明确机型名字的有X86跟N1，x86的填写x86-64或者x86-32根据你编译的填写
- N1的如果有测试，我需要另外的做一份文件
#
---
