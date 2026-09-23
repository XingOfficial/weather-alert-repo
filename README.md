# weather-alert apt 仓库

天气预警查询 App 的 deb 仓库（GitHub Pages 托管）。

## Termux（Android 终端）

```bash
# 添加源
echo "deb [trusted=yes] https://xingofficial.github.io/weather-alert-repo ./" >> $PREFIX/etc/apt/sources.list
apt update
pkg install weather-alert
```

国内可改用镜像加速（gh-proxy）：

```bash
echo "deb [trusted=yes] https://gh-proxy.com/https://xingofficial.github.io/weather-alert-repo ./" >> $PREFIX/etc/apt/sources.list
```

安装后运行 `weather-alert --help`。

## 桌面 Linux（amd64）

```bash
# weather-alert-cli（命令行） / weather-alert-gui（图形界面）
wget https://xingofficial.github.io/weather-alert-repo/weather-alert-cli_1.0.0_amd64.deb
sudo apt install ./weather-alert-cli_1.0.0_amd64.deb
```
