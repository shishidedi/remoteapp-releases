# RemoteApp Updates

RemoteApp 的公开更新发布仓库。

## 更新

0.4.1 及以后版本会从此仓库匿名检查并下载更新，无需 GitHub 账号、邀请或访问令牌。软件启动时及运行期间每 4 小时检查一次，下载完成后由用户点击重启安装。

Release 中的 update ZIP 用于已有部署。首次使用需自行准备 Sunshine、Moonlight 及所需 VPN，并完成网络设置、Sunshine 账号初始化和 PIN 配对。完整组件包目前通过项目所有者的私有部署渠道提供，组件再分发范围见包内 THIRD-PARTY.md。

## 0.4.1

- Tailscale、Radmin VPN、自动选择与手动切换重连四种串流模式。
- 串流参数保存与独立 Moonlight 设置入口。
- 文件传输沿用 Tailscale Taildrop。

自动选路使用连接前端口和延迟探测。实际串流质量需在 Moonlight 中验证。

上游项目包括 Moonlight、Sunshine、Tailscale 和 Radmin VPN，各自适用原项目协议。此仓库中的应用更新包附带相应授权记录。
