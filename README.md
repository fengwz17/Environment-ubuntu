# Environment-ubuntu
ubuntu各种环境配置方法记录

**ubuntu 20.04**

## vscode
### apt安装（测试可行）：
```
sudo apt update
sudo apt install software-properties-common apt-transport-https wget
wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
sudo apt install code
```

### 作为Snap软件包安装（没试过）
```
sudo snap install --classic code
```

## Qv2ray

* https://github.com/Qv2ray/Qv2ray/releases/tag/v2.7.0
* https://github.com/v2ray/v2ray-core/releases/
* 打开Qv2ray: preference(首选项)-内核设置，修改：v2ray-linux-64/v2ray， v2ray-linux-64
* 分组-订阅设置-订阅地址-Basic Base64-更新订阅

## z3
**ubuntu 20.04可以，18.04会有链接问题**
```
sudo apt install z3
```

## yosys
```
sudo add-apt-repository ppa:saltmakrell/ppa
sudo apt-get update
sudo apt-get install yosys
```

## git ssh key
```
git config --global  user.name "用户名"
git config --global user.email "邮箱"
```

生成密钥
```
ssh-keygen -t rsa -C "这里换上你的邮箱"
```

查看id_rsa.pub, $username换成自己的用户名
```
cat /home/$username/.ssh/id_rsa.pub
```

## win10安装ubuntu20.04
* U盘启动盘

1) download [rufus](https://github.com/pbatard/rufus/releases/)
2) download [ubuntu](https://ubuntu.com/download/desktop)
3) follow the default setting in rufus to create the bootable USB flash drives.
