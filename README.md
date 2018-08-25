# 常用一键安装脚本List

## frps

原脚本出处[clangcn](https://github.com/clangcn/onekey-install-shell)。

### Server

安装平台：CentOS、Debian、Ubuntu。

目前脚本安装的版本是**0.21.0**

#### 安装

```Bash
wget --no-check-certificate https://raw.githubusercontent.com/bravecheng/ShellScriptList/master/frps/frps.sh -O ./frps.sh
chmod 700 ./frps.sh
./frps.sh install
```

#### 卸载
```Bash
    ./frps.sh uninstall
```
#### 检查更新
```Bash
    ./frps.sh update
```
#### 管理
```Bash
    /etc/init.d/frps {start|stop|restart|status|config|version}
```

## kcptun

原脚本出处[kuoruan/shell-scripts](https://github.com/kuoruan/shell-scripts)。

### Server

安装平台：CentOS、Debian、Ubuntu。

目前脚本安装的版本是**最新版本**

#### 安装

```Bash
wget --no-check-certificate https://raw.githubusercontent.com/bravecheng/ShellScriptList/master/kcptun/kcptun.sh -O ./kcptun.sh
chmod +x ./kcptun.sh
./kcptun.sh install
```
#### 卸载
```Bash
    ./kcptun.sh uninstall
```
#### 检查更新
```Bash
    ./kcptun.sh update
```
#### 管理
```Bash
	service supervisord {start|stop|restart|status}
    supervisorctl {start|stop|restart|status} kcptun <id>
```

## shadowsocks

原脚本出处[teddysun/shadowsocks_install](https://github.com/teddysun/shadowsocks_install)。

### Server

安装平台:
CentOS: shadowsocks-libev-centos.sh
Debian/Ubuntu: shadowsocks-libev-debian.sh

目前脚本安装的版本是**最新版本**

#### 安装(以debian为例)

```Bash
wget --no-check-certificate -O shadowsocks-libev.sh https://raw.githubusercontent.com/bravecheng/ShellScriptList/master/shadowsocks/shadowsocks-libev-debian.sh
chmod +x shadowsocks-libev.sh
./shadowsocks-libev.sh 2>&1 | tee shadowsocks-libev.log
```
#### 卸载
```Bash
    ./shadowsocks-libev.sh uninstall
```

#### 管理
```Bash
	/etc/init.d/shadowsocks {start|stop|restart|status}
```