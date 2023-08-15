<div align="center">

<h1>StoneOS — 常用插件包合集</h1>

<img src="https://img.shields.io/github/languages/code-size/s71557/StoneOS-Packages?style=for-the-badge&color=32C955"/>
<img src="https://img.shields.io/github/stars/s71557/StoneOS-Packages?style=for-the-badge&color=orange"/>
<img src="https://img.shields.io/github/forks/s71557/StoneOS-Packages?style=for-the-badge&color=ff69b4"/>
<img src="https://img.shields.io/github/license/s71557/StoneOS-Packages?style=for-the-badge&color=blueviolet"/>
</div>

### 项目说明
- StoneOS 常用插件包源码合集，适用于 [lede](https://github.com/coolsnowwolf/lede) 源码

- 自动同步上游源码，一键拉取直接编译，不用再一个个找插件

- SSR Plus+ 依赖全部同步在 `helloworld` 目录内，无需再额外拉取

- PassWall 依赖全部同步在 `openwrt-passwall` 目录内，无需再额外拉取

- 所有插件都为 GITHUB 上收集的开源插件，感谢作者们的付出
  
- 不要Fork本仓库Fork的仓库不会自动同步更新

### 使用方法（以下二选一）
1. 添加到 feeds.conf.default 文件
```yml
sed -i '1i src-git stone https://github.com/s71557/StoneOS-Packages' feeds.conf.default
./scripts/feeds update -a
./scripts/feeds install -a
make menuconfig
```
2. 在源码目录内直接拉取
```yml
git clone https://github.com/s71557/StoneOS-Packages package/StoneOS-Packages
make menuconfig
```

### 插件说明
| 插件 | 说明 |
| ------------- | ------------- |
| helloworld | SSR Plus+ 插件依赖 |
| openwrt-passwall | PassWall 插件依赖 |
| luci-app-openclash | OpenClash 小猫咪科学上网插件 |
| luci-app-passwall | PassWall 科学上网插件 |
| luci-app-passwall2 | PassWall2 科学上网插件 |
| luci-app-ssr-plus | SSR Plus+ 科学上网插件 |
| luci-app-vssr | Hello World 科学上网插件 |
| luci-app-bypass | Bypass 科学上网插件 |
| luci-app-adguardhome | AdGuard Home 去广告 |
| luci-app-smartdns | SmartDNS DNS防污染 |
| luci-app-mosdns | MosDNS DNS转发分流器 |
| luci-app-aliddns | 阿里云 DDNS 插件 |
| luci-app-aliyundrive-fuse | 阿里云盘 Fuse 服务 |
| luci-app-aliyundrive-webdav | 阿里云盘 WebDAV 服务 |
| luci-app-unblockneteasemusic | 解除网易云音乐播放限制 |
| luci-app-quickstart | iStoreOS首页界面 |
| luci-app-store | iStore 应用商店 |
| luci-app-ddnsto | DDNSTO 内网穿透 |
| luci-app-netspeedtest | 网络速度诊断测试 |
| luci-app-dockerman | Docker 图形化插件 |
| luci-app-eqos | IP 限速插件 |
| luci-app-filebrowser | 文件浏览器 |
| luci-app-ikoolproxy | iKoolProxy 滤广告  |
| luci-app-mosdns | DNS 分流解析与广告过滤 |
| luci-app-netdata | 中文版 Netdata 监控 |
| luci-app-oaf | 应用过滤 |
| luci-app-onliner | 在线用户 |
| luci-app-poweroff | 关机 |
| luci-app-pushbot | 全能推送 |
| luci-app-serverchan | 微信推送 |
| luci-app-amlogic | 晶晨宝盒 |
| luci-app-wizard | 设置向导 |
| luci-app-advanced | 系统高级设置 |
| luci-app-wrtbwmon | 流量监控 |
| luci-theme-argon | 老竭力开发的 Argon 主题 |
| luci-app-argon-config | Argon 主题设置，需搭配 Argon 主题使用 |

