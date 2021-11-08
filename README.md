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
