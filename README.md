# **更新内容**
- **添加 WireGuard 解锁 YouTube 选项。**
- **添加节点管理选项，支持删除任意节点的配置，包括服务端与客户端配置文件。**
- **删除节点配置仅支持Version：1.0及之后的版本。**
- **其它优化与修复。**

# **说明**
- **脚本使用sing-box、Juicity内核。**
- **脚本支持 CentOS 8+、Debian 10+、Ubuntu 20+ 操作系统。**
- **脚本所有协议均支持自签证书（NaiveProxy除外）。**
- **脚本支持多用户。**
- **脚本支持所有协议共存。**
- **脚本支持自动续签证书。**

# **安装**
- **Debian&&Ubuntu使用以下命令安装依赖**
```
apt update && apt -y install curl wget tar socat jq git openssl uuid-runtime build-essential zlib1g-dev libssl-dev libevent-dev dnsutils cron
```
- **CentOS使用以下命令安装依赖**
```
yum update && yum -y install curl wget tar socat jq git openssl util-linux gcc-c++ zlib-devel openssl-devel libevent-devel bind-utils cronie
```
- **使用以下命令运行脚本**
```
wget -N -O /root/singbox.sh https://raw.githubusercontent.com/TinrLin/sing-box/main/Install.sh && chmod +x /root/singbox.sh && ln -sf /root/singbox.sh /usr/local/bin/singbox && bash /root/singbox.sh
```

# **使用方法**
- **Clash客户端配置文件位于/usr/local/etc/sing-box/clash.yaml，下载后加载到 Clash 客户端即可使用，需要配合 Meta 内核。**
- **sing-box电脑端配置文件位于/usr/local/etc/sing-box/win_client.json，下载后加载到 V2rayN、SFM 客户端即可使用。**
- **sing-box手机端配置文件位于/usr/local/etc/sing-box/phone_client.json，下载后加载到 SFA、SFI 客户端即可使用。**

# **脚本支持的节点类型**
- **SOCKS**
- **TUIC V5**
- **Juicity**
- **WireGuard--解锁 ChatGPT、Netflix、Disney+**
- **Hysteria2**
- **VLESS+TCP**
- **VLESS+WebSocket**
- **VLESS+gRPC**
- **VLESS+Vision+REALITY**
- **VLESS+H2C+REALITY**
- **VLESS+gRPC+REALITY**
- **Direct--sing-box版任意门**
- **Trojan+TCP**
- **Trojan+WebSocket**
- **Trojan+gRPC**
- **Trojan+TCP+TLS**
- **Trojan+H2C+TLS**
- **Trojan+gRPC+TLS**
- **Trojan+WebSocket+TLS**
- **Hysteria**
- **ShadowTLS V3**
- **NaiveProxy**
- **Shadowsocks**
- **VMess+TCP**
- **VMess+WebSocket**
- **VMess+gRPC**   
- **VMess+TCP+TLS**
- **VMess+WebSocket+TLS** 
- **VMess+H2C+TLS**
- **VMess+gRPC+TLS** 
