# IRMIA 发布产物（releases）

这里**只有安装包**。IRMIA Agent 的源码不在此仓库——本仓库是公开的二进制托管处，只为放发版产物。

## 最新版本：`v0.1.0-beta.12`（Windows x64）

| 类型 | 文件 | 大小 | SHA256 |
| --- | --- | --- | --- |
| 安装包 `installer` | `irmia-agent-v0.1.0-beta.12-win-x64-setup.exe` | 39,721,284 B | `b958fab7d7738ad8d4b10fd77460342040741cc7681f9ad21a5aebeb9a81d9b7` |
| 便携版 `portable` | `irmia-agent-v0.1.0-beta.12-win-x64.zip` | 45,103,215 B | `8667c9e6dfdb388fbd1eb71ca63eee806f72b0b5a4620bb8bcee9b3ed8171567` |

- 下载入口：<https://github.com/irmia2026/irmia-releases/releases>
- 发版清单（客户端据此检查更新，含 `sha256`）：<https://irmia.me/releases/latest.json>
- 发版说明：<https://irmia.me/releases/0.1.0-beta.12/notes.html>

## 拿到文件后先校验

```powershell
Get-FileHash .\irmia-agent-v0.1.0-beta.12-win-x64-setup.exe -Algorithm SHA256
```

与上表逐字比对（大小写不敏感）。**对不上就不要运行。**

## 说明

- 本仓库不含源码、不含配置、不含任何密钥 / 凭据 / 内部文档。
- beta 产物**未做代码签名**，Windows SmartScreen 可能提示"未知发布者"；清单也未签名，`sha256` 只能防传输损坏、不能防篡改。
