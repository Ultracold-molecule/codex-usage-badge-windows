# Codex Usage Badge for Windows

非官方 Windows 用量卡，在 Codex 左侧栏显示 5 小时和每周剩余额度，悬停可查看重置时间。

**实验版**：已在一台已登录的 Windows Store 版 Codex 上验证圆环显示。后台监督进程曾在一次重启中退出，多次重启、其他电脑及未来客户端版本尚未充分验证。

## 安装

需要 Windows 10/11、已登录的 Codex 桌面客户端和 Node.js 24 或更高版本。

1. 点击仓库页面 **Code → Download ZIP**，完整解压。
2. 双击 `Install.cmd`。保存工作并完全退出 Codex。
3. 从原来的 Codex 图标打开，稍等片刻。后台可能正常重开一次客户端；如果启动后立即操作，保护机制可能跳过加载。

`Status.cmd` 查看诊断，`Uninstall.cmd` 卸载。安装位置为当前用户的 Documents 目录。此版本不自动更新，请手动获取本仓库的新版本。

插件使用本机 39222 调试接口，本机其他程序也可能访问该接口，请勿转发或对外开放。客户端内部接口或界面变化可能导致失效。详情见 [Windows 安装与限制](README-Windows.md)。

基于 [jaykinhoo9/codex-usage-badge](https://github.com/jaykinhoo9/codex-usage-badge) 的 Windows 启动代码及 [Lorie7813/codex-usage-card](https://github.com/Lorie7813/codex-usage-card) 的额度圆环，保留 [MIT 许可证](LICENSE)。本项目与 OpenAI 无官方关联。

An experimental, unofficial Windows sidebar badge for Codex remaining usage. See [installation and limitations](README-Windows.md).
