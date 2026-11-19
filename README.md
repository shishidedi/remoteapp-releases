# RemoteApp

Windows x64 双向远程桌面控制 APP，组合 Sunshine、Moonlight 及 Tailscale 或 Radmin VPN。

## 下载和首次使用

进入本仓库 Releases，选择最新正式版本的 `RemoteApp-<版本>-win-x64-full.zip`，用同页 SHA256SUMS.txt 核对哈希后完整解压，运行 RemoteApp.exe。

APP 自带 .NET 运行时。第三方软件通过 APP 内的官方下载按钮或包内 README.md 提供的链接安装。两端准备 Sunshine、Moonlight 及所需 VPN，完成组网、Sunshine 账号设置及 PIN 配对。

| 组件 | 官方下载 |
|---|---|
| Sunshine | https://github.com/SunshineStream/Sunshine/releases/latest |
| Moonlight | https://github.com/moonlight-stream/moonlight-qt/releases/latest |
| Tailscale | https://tailscale.com/download/windows |
| Radmin VPN | https://www.radmin-vpn.com/ |
| VC++ x64 运行库 | https://learn.microsoft.com/cpp/windows/latest-supported-vc-redist |

## 功能与更新

- Tailscale、Radmin VPN、自动选择与手动切换重连四种串流模式。
- APP 内串流参数保存及独立 Moonlight 设置入口。
- 文件传输使用 Tailscale Taildrop，沿用既有同账号设备模式。
- 匿名检查及下载更新，无需 GitHub 登录或访问邀请。启动时及运行期间每 4 小时检查，下载完成后点击重启安装。

`update.zip` 用于已有部署，`full.zip` 用于首次部署。第三方软件适用各自协议并通过官方渠道更新。自动选路依据连接前端口与延迟探测，实际串流效果请在 Moonlight 中验收。
