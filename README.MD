 ######### v2ray
最好用的 V2Ray 一键安装脚本 &amp; 管理脚本

功能特点

    支持 V2Ray 多数传输协议
    支持 WebSocket + TLS / HTTP/2
    支持 动态端口 (WebSocket + TLS，Socks5， HTTP/2 除外)
    支持 屏蔽广告
    支持 配置 Shadowsocks
    支持 下载客户端配置文件 (不用 Xshell 也可以下载)
    客户端配置文件同时支持 SOCKS 和 HTTP
    支持 生成 V2Ray 配置二维码链接 (仅适用部分客户端)
    支持 生成 V2Ray 配置信息链接
    支持 生成 Shadowsocks 配置二维码链接
    支持修改 V2Ray 传输协议
    支持修改 V2Ray 端口
    支持修改 动态端口
    支持修改 用户ID
    支持修改 TLS 域名
    支持修改 Shadowsocks 端口
    支持修改 Shadowsocks 密码
    支持修改 Shadowsocks 加密协议
    自动启用 BBR 优化 (如果内核支持)
    集成可选安装 BBR (by teddysun.com)
    集成可选安装 锐速 (by moeclub.org)
    一键 查看运行状态 / 查看配置信息 / 启动 / 停止 / 重启 / 更新 / 卸载 / 等等…
    人性化向导 & 纯净安装 & 卸载彻底

哈哈哈..我故意要写够 23 条的。说着当然，脚本肯定都会有如上所说的功能。
安装或卸载

要求：Ubuntu 14+ / Debian 7+ / CentOS 7+ 系统的小鸡鸡
推荐使用 Debian 9 系统，脚本会自动启用 BBR 优化。
备注：不推荐使用 Debian 8 系统，因为 Caddy 申请证书可能会出现一些莫名其妙的问题
强烈推荐使用 搬瓦工VPS，稳定，快速，针对中国线路专门优化，完全无须担心跑路，服务好，30天退款保证。
在这里可以找到 搬瓦工 VPS 优惠码
使用 root 用户输入下面命令安装或卸载

##### bash <(curl -s -L https://233yes.com/v2ray.sh) 

    如果提示 curl: command not found ，那是因为你的 VPS 没装 Curl
    ubuntu/debian 系统安装 Curl 方法: apt-get update -y && apt-get install curl -y
    centos 系统安装 Curl 方法: yum update -y && yum install curl -y
    安装好 curl 之后就能安装脚本了

注意事项：如果你是 CentOS 7 系统，此脚本会关闭 firewalld 并且使用 iptables
备注：安装完成后，输入 v2ray 即可管理 V2Ray
如果提示你的系统不支持此脚本，那么请尝试更换系统

快速管理

 ### v2ray info 查看 V2Ray 配置信息
 ### v2ray config 修改 V2Ray 配置
 ### v2ray link 生成 V2Ray 配置文件链接
 ### v2ray infolink 生成 V2Ray 配置信息链接
 ### v2ray qr 生成 V2Ray 配置二维码链接
 ### v2ray ss 修改 Shadowsocks 配置
 ### v2ray ssinfo 查看 Shadowsocks 配置信息
 ### v2ray ssqr 生成 Shadowsocks 配置二维码链接
 ### v2ray status 查看 V2Ray 运行状态
 ### v2ray start 启动 V2Ray
 ### v2ray stop 停止 V2Ray
 ### v2ray restart 重启 V2Ray
 ### v2ray log 查看 V2Ray 运行日志
 ### v2ray update 更新 V2Ray
 ### v2ray update.sh 更新 V2Ray 管理脚本
 ### v2ray uninstall 卸载 V2Ray

配置文件路径

 ### V2Ray 配置文件路径：/etc/v2ray/config.json
 ### Caddy 配置文件路径：/etc/caddy/Caddyfile
 ### 脚本配置文件路径: /etc/v2ray/233blog_v2ray_backup.conf

    警告，请不要修改脚本配置文件，免得出错。。
    如果你不是有特别的需求，也不要修改 V2Ray 配置文件
    不过也没事，若你实在想要瞎折腾，出错了的话，你就卸载，然后重装，再出错 ，再卸载，再重装，重复到自己不再想折腾为止。。

备注

V2Ray 客户端配置文件 SOCKS 监听端口为 2333， HTTP 监听端口为 6666
可能某些 V2Ray 客户端的选项或描述略有不同，但事实上，此脚本显示的 V2Ray 配置信息已经足够详细，由于客户端的不同，请对号入座。

