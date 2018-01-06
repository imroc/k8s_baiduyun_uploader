# k8s_baiduyun_uploader
下载kubernetes相关文件并上传到百度云，基于[bpcs_uploader](https://github.com/oott123/bpcs_uploader)

# 系统要求
Linux (or cygwin) with php & curl installed.

# 使用方法
初始化：
``` sh
./bpcs_uploader.php quickinit
```
敲下命令直接进入快速初始化流程，输入y，然后打开浏览器访问 https://openapi.baidu.com/device ，在“请输入设备上显示的用户授权码：”文本框中输入上面显示的授权码（如12abcxyz），并点击继续。 看到网页上显示“请返回设备继续操作！”后，返回ssh上按下回车后，即完成了初始化配置。


上传k8s:
``` sh
./upload 1.9.1
```
它会下载kuernetes相关文件然后上传到你的网盘路径：`我的应用数据/bpcs_uploader/1.9.1/1` (前提是你服务器的所在的网络能够下载到kubernetes的文件)

