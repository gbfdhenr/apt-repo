# GBfdHenr APT 仓库

## 当前应用

| 应用 | 版本 | 架构 | 作者 | 描述 |
|------|------|------|------|------|
| mini-browser | 1.0.0 | amd64 | gbfdhenr | 基于 PyQt6 + QtWebEngine 的轻量级网页浏览器 |

## 使用方式

```bash
# 导入 GPG 公钥
sudo mkdir -p /etc/apt/keyrings
sudo curl -fsSL https://raw.githubusercontent.com/gbfdhenr/apt-repo/master/gpg.gpg \
  -o /etc/apt/keyrings/gbfdhenr.gpg

# 添加源
echo "deb [signed-by=/etc/apt/keyrings/gbfdhenr.gpg arch=amd64] https://raw.githubusercontent.com/gbfdhenr/apt-repo/master gbfdhenr main" \
  | sudo tee /etc/apt/sources.list.d/gbfdhenr.list

# 更新并安装
sudo apt update
sudo apt install mini-browser
```
