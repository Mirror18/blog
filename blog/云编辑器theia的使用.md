# 云编辑器theia的使用

## 电脑配置

先链接服务器用于上传和下载文件

### 服务器连接

本地与云服务器进行数据对接.这里选用ssh登陆,

### ssh链接云服务器

0. 无法登陆的常见问题[云服务器 Linux 实例：无法通过 SSH 方式登录-故障处理-文档中心-腾讯云 (tencent.com)](https://cloud.tencent.com/document/product/213/37925)

1. 下载私钥https://mirrorcloud.lanzoul.com/iE6kG0zrouqd
2. 解压缩,放到![image-20230622220659431](https://raw.githubusercontent.com/jerry857/iamge/main/image-20230622220659431.png)这个地方,如果没有自己创建文件夹也成
3. 打开powershell, `ctrl`+`r`输入`powershell`![image-20230622220843075](https://raw.githubusercontent.com/jerry857/iamge/main/image-20230622220843075.png)
4. 输入`ssh ubuntu@81.71.49.23`回车
5. 如果遇到需要输入yes的直接输入yes即可
6. 密码`Makai2001`![image-20230622221317170](https://raw.githubusercontent.com/jerry857/iamge/main/image-20230622221317170.png)
7. 登陆完成,至于如何上传和下载文件,这个没有研究过,我一般都是用的gitee或者github.需要使用的文件都在云端,需要的时候就git clone就完事了.这个需要自己研究如何上下传文件.
8. [WinSCP :: Official Site :: Free SFTP and FTP client for Windows](https://winscp.net/eng/index.php)这个软件是Windows和服务器文件传输用的,这个我没用过,可以自行查看这里面的文档文档

## theia的使用

### 登陆

1. 浏览器输入这个网址http://81.71.49.23/
2. 账号 `admin`
3. 密码 `makai2001`

![image-20230622221944072](https://raw.githubusercontent.com/jerry857/iamge/main/image-20230622221944072.png)

登陆成功

### theia的使用

其实这玩意儿跟`vscode`一样..创建和使用也一样,除了是英文的,不过也有解决办法,但这个我没时间搞了,.

1. 点击`open workspace`![image-20230622222709749](https://raw.githubusercontent.com/jerry857/iamge/main/image-20230622222709749.png)先确定好工作空间
2. ![image-20230622222833005](https://raw.githubusercontent.com/jerry857/iamge/main/image-20230622222833005.png)都放在`data`文件下,再新建一个`folder`,把资料都放到这里.`mirror`的文件是我现在在使用
3. 就可以用新建文件写东西了
4. ![image-20230622223427553](https://raw.githubusercontent.com/jerry857/iamge/main/image-20230622223427553.png)点这里运行.没反应就用命令行执行.

### 下载插件

![image-20230622223518981](https://raw.githubusercontent.com/jerry857/iamge/main/image-20230622223518981.png)这个就是,但现在有问题,关于国内访问国外网站的事.下载不下来。下一个篇章说解决办法.这也是说为什么这玩意是英文的,中文插件下载不下来啊.

## 云服务器配置

从这一步就要开始全程使用国外的网络。很显然这些文档国内都访问不了。

### theia的使用配置

https://theia-ide.org/docs/user_toolbar这个网站就是关于他的使用文档.可以在这里面了解各种问题.现在也是成熟的发型版本,应该说是问题不大

### 关于网络的配置

1. 本地网络,需要点科学.这个只能使用clash,

https://github.com/Fndroid/clash_for_windows_pkg/releases这里面都是他的发行版本,根据不同的系统选择不同的版本.

Windows是有UI界面的，随便一搜都有教程。

2. 云服务器端的网络配置。这个也需要下载clash，但因为服务器部分没有配置桌面，所以没有办法直接使用，需要解压后`tar zxvf 包名.tar.gz`进入里面直接使用.
3. 没有时间,所以这里就放上clash的官方文档。https://dreamacro.github.io/clash/