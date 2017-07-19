# DigitalOcean 配置Shadowsocks的方法

## 创建Droplets
创建ssh密钥

## 安装必要软件
由于shadowsocks需要从pip源安装，因此对于一个干净的droplet来说，要先安装一些必要的软件

用ssh连接vps：

```shell
ssh root@your_droplet_ip
```


安装python

```shell
apt install python
```

安装pip

```shell
wget https://bootstrap.pypa.io/get-pip.py
python get-pip.py
```

安装shadowsocks
pip install shadowsocks

```json
{
    "server": "<Your server IP>",
    "server_port": 8388,
    "local_address": "127.0.0.1",
    "local_port": 1080,
    "password": "<Your password>",
    "timeout": 300,
    "method": "aes-256-cfb",
    "fast_open": false
}
```
~. 关闭ssh

## 关于DigitalOcean
收费

机房

维护

## 各平台下的客户端
