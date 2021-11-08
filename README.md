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
