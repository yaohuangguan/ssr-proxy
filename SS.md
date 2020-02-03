开始搭建ss
连接到你的 vultr 服务器之后，接下来就可以使用几个命令让你快速搭建一个属于自己的 ss 服务器：

输入以下命令，然后回车：
 yum install wget
接着执行安装shadowsocks：
wget –no-check-certificate -O shadowsocks.sh https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks.sh
获取 shadowsocks.sh 读取权限：
chmod +x shadowsocks.sh
设置你的 ss 密码和端口号：
输入./shadowsocks.sh 2>&1 | tee shadowsocks.log后就可以设置密码和端口号了：

设置密码

选择加密方式
设置完密码和端口号之后，我们选择加密方式，这里选择 7 ，使用aes-256-cfb的加密模式： vultr ss服务器 接着按任意键进行安装。

安装ss完成
等一会之后，就安装完成了，它会给你显示你需要连接 vpn 的信息： vultr ss服务器 可以看到需要连接 ss 的 ip地址，密码，端口，和加密方式。

搞定，将这些信息保存起来，那么这时候你就可以使用它们来科学上网啦。
安装 BBR
wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh
获取读写权限
chmod +x bbr.sh
启动BBR安装
./bbr.sh