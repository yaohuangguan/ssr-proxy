# ssr-proxy

安装 git
输入命令：
yum install git

下载安装ssr安装脚本
输入命令：
yum install wget
输入命令：
wget –no-check-certificate -O ss-fly.sh https://raw.githubusercontent.com/flyzy2005/ss-fly/master/ss-fly.sh

运行ssr脚本
输入命令：
chmod +x ss-fly.sh
输入命令：
ss-fly.sh -ssr

运行之后会提示你输入密码：

1
2
Please enter password for ShadowsocksR:
(Default password: teddysun.com) : (在这里输入密码然后回车)
接着会提示你输入端口号：

1
Please enter a port for ShadowsocksR [1-65535] (Default port: 14593):(在这里输入端口然后回车)
接着会提示你输入加密方式：

1
Please select stream cipher for ShadowsocksR:（这里输入 7 然后回车）
最后就会出现下面的内容，说明你已经安装ssr成功了：

1
2
3
4
5
6
7
8
9
10
Congratulations, ShadowsocksR server install completed!
Your Server IP        :服务器ip
Your Server Port      :端口
Your Password         :密码
Your Protocol         :协议
Your obfs             :混淆
Your Encryption Method:your_encryption_method

Welcome to visit:https://shadowsocks.be/9.html
Enjoy it!
SSR 命令操作
启动：/etc/init.d/shadowsocks start
停止：/etc/init.d/shadowsocks stop
卸载：./shadowsocksR.sh uninstall
一键开启 BBR 加速
到这里你是安装成功SSR了，不过还可以加速上网：

1
ss-fly/ss-fly.sh -bbr
然后会提示你重启才会生效，我们按【y】进行重启。

这样就可以了。