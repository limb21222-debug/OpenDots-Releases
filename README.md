# OpenDots Windows 发行版

此仓库只发布编译后的 Windows 程序、更新清单与使用说明，不保存 OpenDots 项目源码或使用者的数据。

## 下载与首次使用

请在 [Releases 最新正式版](https://github.com/limb21222-debug/OpenDots-Releases/releases/latest) 中下载 `OpenDots-Windows-x64.zip`，完整解压到可写目录后双击 `OpenDots.exe`。支持 Windows 10/11 x64，已包含 Node.js 运行时。

每位使用者自行配置账号、代理、Hub 环境及模型密钥；需要安装 Google Chrome。首次启动不包含预置账号、Cookie、模型密钥或运营记录。详细步骤见压缩包内的 `使用说明.txt`。

## 程序内更新

187 版起默认连接本仓库。在“设置 → 程序更新”检查新版、查看发布说明、下载并确认安装；旧版可将更新仓库填写为 `limb21222-debug/OpenDots-Releases`。自动检查不会自动安装，无需登录 GitHub。

新版支持下载进度、暂停与断点续传，并校验包大小、SHA-256 和逐文件清单。安装前安全暂停运营，安装后重启并核对实际版本，运营保持暂停。安装或启动失败时尝试恢复原版本与安装前数据库，并显示实际结果。

本机账号、浏览器登录资料、模型密钥和运营进度保留在安装目录的 `data` 与 `.local`，请妥善备份。向他人分发时请使用 Releases 原始 ZIP，不要压缩自己已经配置过的安装目录。

## 发布内容

- `OpenDots-Windows-x64.zip`：完整编译程序与必要运行库。
- `update.json`：版本号、文件名、大小和 SHA-256，供程序检查更新。
- `SHA256SUMS.txt`：供手动核对下载文件。

每个正式版使用独立版本号与标签。本机维护版本和 GitHub 发布使用同一份编译产物。

GitHub 自动生成的“Source code”压缩包只包含本仓库的说明文件，不包含 OpenDots 项目源码；请下载上面的 Windows ZIP。编译后的 JavaScript 与必要第三方运行库属于程序文件，不提供防逆向保证。
