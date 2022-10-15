# manjaro snap 方式安装软件
### 安装snap

```
sudo pacman -S snapd
sudo systemctl enable --now snapd.socket
sudo ln -s /var/lib/snapd/snap /snap
```

#### 安装 slack
```
sudo snap install slack
```

### 安装sublime text 
```
sudo snap install sublime-text --classic
```