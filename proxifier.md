# Shadowsocks 配合 Proxifier 实现客戶端代理

## 什么是 Proxifier

Proxifier 是一款功能非常強大的socks5客戶端，可以让不支持通过代理服务器工作的网络程序能通过HTTPS或SOCKS代理或代理链。支持64位系統，支持 XP，Vista，Win7，MacOS, 支持socks4，socks5，http代理协议，支持TCP，UDP协议，可以指定端口，指定 IP，指定域名,指定程序等运行模式，兼容性非常好，和 SOCKSCAP 属于同类软件，不过SOCKSCAP已经很久没更新了，不支持64位系統。有许多网络應应用程序不支持通过代理服务器工作，Proxifier解决了这些问题和所有限制，让您有机会不受任何限制使用你喜爱的软件。此外，它让你获得了额外的网络安全控制，创建代理隧道，並添加使用更多网络功能的权力。

## 使用方法

### Proxifier 下載

官网下载地址：[点击这里](http://www.proxifier.com/download/)

#### Windows 版本

软件分为 Standard Edition 和 Portable Edition 版本，请自行购买注册码

#### MacOS 版本

请自行购买注册码

若系统为 10.11，请下载[Beta版 ](http://www.proxifier.com/download/ProxifierMac.dmg)

若Yosemite下Proxifier不能运行，打开 终端 应用，运行下面的命令然后重启

```
sudo nvram boot-args="kext-dev-mode=1"
```

#### 详细使用方法：

因为 Windows 和 MacOS 的使用方式是一样的，这里就只演示 MacOS 下的使用方法

首先点击 `proxies` > `add`

在其中填写 `socks5` 的代理地址 `127.0.0.1:1080` 请确保与图中一致

![](/img/proxifier1.jpg)
![](/img/proxifier2.jpg)

接下來填写代理规则

![](/img/proxifier3.jpg)

最重要的就是请将Shadowsocks客戶端设置为全局模式

如图，点击*+* 添加 APP，再在 `Action` 中选择 `Direct`

![](/img/proxifier4.jpg)

此时就可以添加其他 APP 了，比如让 Steam 和 CS:GO 走 Shadowsocks 以降低延时，那么如图：

![](/img/proxifier5.jpg)

确保选择的是走 `socks5` 就可以了

#### [<< 返回首页](https://super-ssr.github.io/Shadowsocks/)
