# OpenWrt x86_64 24.10.1 编译模板

纯官方 OpenWrt 24.10.1（x86_64，内核6.12.33），集成 LuCI 和基础防火墙，一键 Fork 即可编译。

## 🧾 使用说明

1. Fork 或新建仓库，将本模板内容添加；
2. 如需 Telegram 通知，请在仓库 Settings → Actions → Secrets 中添加：
   - `TELEGRAM_BOT_TOKEN`
   - `TELEGRAM_CHAT_ID`
3. 前往 GitHub → Actions → 运行 “Build OpenWrt 24.10.1 x86_64”；
4. 构建完成后，可在 Artifacts 或 Releases 下载固件；
5. 使用 `*.img.gz` 镜像文件刷写设备即可。

## 🔧 可选修改

- 如需 WireGuard 支持，请取消 `config/minimal.config` 对应注释；
- 若需自定义功能/插件，可编辑 `.config` 或 feeds 源；
- 如希望自动定时构建，请在 workflow 中改为 `schedule` 触发器。

---

感谢使用！欢迎提交 Issue 和 PR 进行模板优化 😊
