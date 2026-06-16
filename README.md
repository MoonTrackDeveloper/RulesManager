[English](#english) · [简体中文](#简体中文)

---

## English

Desktop client for managing AI coding tool rule files (Cursor, Trae, OpenCode, and more) on **Windows** and **macOS**.

> **Proprietary software** — This repository contains installers and documentation only. **No source code.** By downloading or installing, you agree to the [License](LICENSE). Installers are published by **MoonTrackDeveloper** on GitHub.

> **Download only from [Releases on this repository](https://github.com/MoonTrackDeveloper/RulesManager/releases/latest)** — do not use third-party mirrors or repacks.

**[Download latest →](https://github.com/MoonTrackDeveloper/RulesManager/releases/latest)**

| File | Platform | Description |
|------|----------|-------------|
| `Rules Manager_*_x64-setup.exe` | Windows 10/11 x64 | NSIS installer |
| `Rules Manager_*_aarch64.dmg` | macOS 11+ (Apple Silicon) | DMG with `.app` |

### Install — Windows

1. Download `*-setup.exe` from [Releases](https://github.com/MoonTrackDeveloper/RulesManager/releases/latest)
2. Run the installer and complete the wizard
3. Launch **Rules Manager** from the Start menu

### Install — macOS (Apple Silicon)

1. Download `*_aarch64.dmg` from [Releases](https://github.com/MoonTrackDeveloper/RulesManager/releases/latest)
2. Open the DMG; accept the license if prompted, then drag **Rules Manager** to Applications
3. Launch from Applications (or Spotlight)

**Intel Mac (x86_64)** is not supported in this release channel.

### SmartScreen (Windows)

Installers are not code-signed. If you see "Unknown publisher", choose **More info** → **Run anyway**. Download only from Releases on this repository.

### Gatekeeper (macOS)

Installers are **not notarized or code-signed**. On first launch, macOS may block the app. Open **System Settings → Privacy & Security**, find the blocked-app message, and choose **Open Anyway** (or right-click the app → **Open** once). Download only from Releases on this repository.

### Data & Privacy

Rules Manager does **not** collect telemetry, crash reports, or analytics. It never contacts the developer's servers. No account registration or advertising IDs. Rule files and app settings are stored locally. The only network access is to **Git remotes you configure**. Git authentication uses your system's OpenSSH agent (**SSH**, default) or **git credential helper** (**HTTPS**); this app does **not** store private keys or tokens. `git_config.json` only saves remote URL and auth mode under the rule library folder. Use minimal-scope HTTPS tokens if applicable. You are responsible for backing up your rule files and securing your Git credentials.

### Data & uninstall

| Path | Contents |
|------|----------|
| **Windows** `%USERPROFILE%\.rules-manager\` | Rule library (kept after uninstall) |
| **Windows** `%APPDATA%\.rules-manager\` | App database & preferences |
| **macOS** `~/.rules-manager/` | Rule library (kept after uninstall) |
| **macOS** `~/Library/Application Support/.rules-manager/` | App database & preferences |
| **Linux** `~/.rules-manager/` | Rule library |
| **Linux** `~/.local/share/.rules-manager/` | App database & preferences |

Uninstall: **Windows** — Settings → Apps → Rules Manager → Uninstall. **macOS** — drag **Rules Manager** from Applications to Trash (rule library under `~/.rules-manager/` is kept).

### Organization / bulk deployment

The [license](LICENSE) grants **personal use** only. For company-wide or bulk deployment, open a [GitHub Issue](https://github.com/MoonTrackDeveloper/RulesManager/issues) to discuss — do not assume team Git sync implies a site license.

© 2026 [MoonTrackDeveloper](https://github.com/MoonTrackDeveloper) · [License](LICENSE) (proprietary) · [Third-party notice](NOTICE.md) (bundled open source libraries only, not this app's source code)

---

## 简体中文

统一管理 Cursor、Trae、OpenCode 等 AI 编程工具规则文件的 **Windows / macOS** 桌面客户端。

> **专有软件** — 本仓库仅含安装包与说明文档，**不含源代码**。下载或安装即表示您同意 [软件许可协议](LICENSE)。安装包由 **MoonTrackDeveloper** 在 GitHub 个人发布。

> **请仅从 [本仓库 Releases](https://github.com/MoonTrackDeveloper/RulesManager/releases/latest) 下载** — 勿使用第三方网盘、群聊转发的安装包。

**[下载最新版 →](https://github.com/MoonTrackDeveloper/RulesManager/releases/latest)**

| 文件 | 平台 | 说明 |
|------|------|------|
| `Rules Manager_*_x64-setup.exe` | Windows 10/11 x64 | NSIS 安装包 |
| `Rules Manager_*_aarch64.dmg` | macOS 11+（Apple Silicon） | DMG（含 `.app`） |

### 安装 — Windows

1. 从 [Releases](https://github.com/MoonTrackDeveloper/RulesManager/releases/latest) 下载 `*-setup.exe`
2. 双击运行并完成向导
3. 从开始菜单启动 **Rules Manager**

### 安装 — macOS（Apple Silicon）

1. 从 [Releases](https://github.com/MoonTrackDeveloper/RulesManager/releases/latest) 下载 `*_aarch64.dmg`
2. 打开 DMG；若提示许可协议请阅读并同意，将 **Rules Manager** 拖入「应用程序」
3. 从「应用程序」或 Spotlight 启动

**Intel Mac（x86_64）** 暂不提供本渠道安装包。

### SmartScreen（Windows）

安装包尚未代码签名。若提示「未知发布者」，点 **更多信息** → **仍要运行**。请仅从本仓库 Releases 下载。

### Gatekeeper（macOS）

安装包**未经公证或代码签名**。首次打开时 macOS 可能拦截。请在 **系统设置 → 隐私与安全性** 中找到被阻止提示并选择 **仍要打开**（或右键应用 → **打开** 一次）。请仅从本仓库 Releases 下载。

### 数据与隐私

本应用**不**收集遥测、崩溃上报或分析数据，也**不会**连接开发者服务器。无需注册账户，无广告标识符。规则与应用数据均保存在本机（路径见下表）。唯一网络访问为**你配置的 Git 远程**。Git 认证通过系统 OpenSSH / ssh-agent（**SSH**，默认）或 **git credential helper**（**HTTPS**）完成；本应用**不**保存私钥或令牌。`git_config.json` 仅保存远程地址与认证方式（位于规则库目录）。使用 HTTPS 时请采用最小权限令牌。规则文件备份与 Git 凭证安全由你自行负责。

### 数据与卸载

| 路径 | 内容 |
|------|------|
| **Windows** `%USERPROFILE%\.rules-manager\` | 规则库（卸载后保留） |
| **Windows** `%APPDATA%\.rules-manager\` | 应用数据库与偏好 |
| **macOS** `~/.rules-manager/` | 规则库（卸载后保留） |
| **macOS** `~/Library/Application Support/.rules-manager/` | 应用数据库与偏好 |
| **Linux** `~/.rules-manager/` | 规则库 |
| **Linux** `~/.local/share/.rules-manager/` | 应用数据库与偏好 |

卸载：**Windows** — 设置 → 应用 → Rules Manager → 卸载。**macOS** — 将「应用程序」中的 **Rules Manager** 拖入废纸篓（`~/.rules-manager/` 规则库保留）。

### 组织 / 批量部署

[许可协议](LICENSE) 仅授予**个人使用**。若需公司内统一安装或批量部署，请通过 [GitHub Issues](https://github.com/MoonTrackDeveloper/RulesManager/issues) 联系 — 勿将 Git 协作同步理解为站点授权。

© 2026 [MoonTrackDeveloper](https://github.com/MoonTrackDeveloper) · [软件许可协议](LICENSE)（专有）· [第三方组件声明](NOTICE.md)（仅指内置开源库，非本软件源码）
