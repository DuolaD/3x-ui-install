# 3x-ui-install 🚀

本仓库是 [3x-ui](https://github.com/MHSanaei/3x-ui) 的增强版一键安装脚本项目。在官方原版安装脚本的基础上，提供了一些实用的增强功能（例如：跳过 SSL 设置、支持一键生成自签名 SSL 证书等）。

---

## ⚡ 快速安装

您可以通过以下命令，直接复制并在终端运行来进行一键安装：

```bash
bash <(curl -Ls https://raw.githubusercontent.com/DuolaD/3x-ui-install/main/install.sh)
```

### 📌 安装特定版本
如果您需要安装特定的 3x-ui 版本（例如 `v2.4.0`），可以在命令后加上版本号：

```bash
bash <(curl -Ls https://raw.githubusercontent.com/DuolaD/3x-ui-install/main/install.sh) v2.4.0
```

### 📌 安装开发版 (Dev Build)
要安装滚动更新的最新的测试版本，请在命令后加上 `dev-latest`：

```bash
bash <(curl -Ls https://raw.githubusercontent.com/DuolaD/3x-ui-install/main/install.sh) dev-latest
```

---

## 🌟 增强功能特性

相比于官方原版安装脚本，本项目做出了以下定制和优化：

1. **🔒 一键生成自签名 SSL 证书**
   - 在安装交互中，支持直接选择生成并配置自签名的 SSL 证书，无需繁琐地去申请或配置外部证书，即可快速启用 HTTPS 加密访问。
2. **⏭️ 跳过 SSL 交互设置**
   - 支持在安装流程中快速跳过 SSL 相关的设置，以满足希望后期手动配置或使用纯 HTTP 访问的用户需求。
3. **📁 完整的自定义脚本分发**
   - 所有的辅助管理脚本 (`x-ui`)、更新脚本 (`update.sh`) 及系统服务文件均托管于本仓库，确保您后续运行 `x-ui` 面板控制命令时，始终运行的是来自本仓库的定制优化版本，而不会被官方原版重置。

---

## 🛠️ 管理菜单使用说明

安装成功后，在服务器终端输入 `x-ui` 即可进入管理菜单：

| 命令 | 描述 |
| :--- | :--- |
| `x-ui` | 打开面板管理菜单 (交互式) |
| `x-ui start` | 启动 x-ui 面板 |
| `x-ui stop` | 停止 x-ui 面板 |
| `x-ui restart` | 重启 x-ui 面板 |
| `x-ui status` | 查看 x-ui 面板状态 |
| `x-ui settings` | 查看当前面板配置参数 |
| `x-ui enable` | 开启 x-ui 开机自启 |
| `x-ui disable` | 关闭 x-ui 开机自启 |
| `x-ui log` | 查看面板日志 |
| `x-ui update` | 更新面板组件到本项目的最新版本 |
| `x-ui uninstall` | 卸载 x-ui 面板 |

---

## 🔗 相关项目

- 官方 3x-ui 仓库：[MHSanaei/3x-ui](https://github.com/MHSanaei/3x-ui)

## 〢 贡献者

- [哆啦D夢|DuolaD](https://github.com/DuolaD)