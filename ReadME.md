# 竞斗云插件宝库

### 注意：本插件库为 Lean OPENWRT 版的 竞斗云(PW_R619AC) 定制，当然也支持任何 armv7 系统。

### 使用方法：
- 首先你得有个干净的固件，没有的往 [这里](https://github.com/kiss2u/Lean-Actions/releases) 看，选一个以 **openwrt-ipq40xx-p2w_r619ac-128m-xxx** 开头的固件下载后安装。
- 在浏览器输入 192.168.100.3，用户名 root ，密码为 password 登录系统，选择 **系统** -> **文件传输** -> **上传**，选择 ipk，确定上传。
- 该页面往下拉，看到上传成功后的文件，依次点击安装，完成之后刷新页面即可。

### Q&A
- 安装失败怎么办？
- ssh 方式登录固件后台，进入 '/tmp/upload/' 目录，可以看到上传的 ipk 文件，输入命令 opkg install xxx.ipk 安装。
- 还是失败怎么办？
- 输入 uname -a，查看你的系统架构，若非 **armv7** 系统，就不要折腾了。
