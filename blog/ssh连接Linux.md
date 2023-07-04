# ssh连接Linux

## 服务器连接

本地与云服务器进行数据对接.这里选用ssh登陆,

### ssh链接云服务器

0. 无法登陆的常见问题[云服务器 Linux 实例：无法通过 SSH 方式登录-故障处理-文档中心-腾讯云 (tencent.com)](https://cloud.tencent.com/document/product/213/37925)

1. 下载私钥
2. 解压缩,放到![image-20230622220659431](https://raw.githubusercontent.com/jerry857/iamge/main/image-20230622220659431.png)这个地方,如果没有自己创建文件夹也成.同时也是说其他设备想要远程登陆的话,也是需要这个私钥放到ssh上,所以Linux登陆Linux同理.
3. 打开powershell, `ctrl`+`r`输入`powershell`![image-20230622220843075](https://raw.githubusercontent.com/jerry857/iamge/main/image-20230622220843075.png)
4. 输入`ssh ubuntu@xxx.xxx.xxx.xxx`回车,ps(我的服务器是ubuntu的,默认名字,有可能有不同的名字)
5. 如果遇到需要输入yes的直接输入yes即可
6. 密码`xxxxx`![image-20230622221317170](https://raw.githubusercontent.com/jerry857/iamge/main/image-20230622221317170.png)
7. 登陆完成,至于如何上传和下载文件,这个没有研究过,我一般都是用的gitee或者github.需要使用的文件都在云端,需要的时候就git clone就完事了.这个需要自己研究如何上下传文件.

