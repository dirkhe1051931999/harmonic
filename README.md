# harmonic

个人 Codex 第三方 Skill 库，存放用于备份和同步的副本。

## 在 Codex 中使用

在 Codex 聊天输入框里发送 `$技能名 任务描述`。也可以直接说「请用 humanizer-zh 润色下面的正文」。在 Codex CLI 或 IDE 扩展中，可输入 `/skills` 查看可用技能，或键入 `$` 选择。

在新电脑上，把要用的整个 Skill 文件夹复制到 Codex 的用户 Skill 目录，例如 Windows 上的 `%USERPROFILE%\.codex\skills\`（本机当前使用的目录）。保留文件夹内的 `SKILL.md` 和配套资源。如果复制后看不到技能，重启 Codex。

## 写作与回复

- [caveman](./caveman/SKILL.md) 精简对话回复，保留命令、路径和技术细节。发送 `$caveman 接下来的回复简短一点`，恢复时发送「退出 caveman 模式」。
- [humanizer-zh](./humanizer-zh/SKILL.md) 润色已有中文稿件，保留原文事实和作者语气。发送 `$humanizer-zh 润色下面这段正文，保留技术细节`，再附上原文。
- [content-research-writer](./content-research-writer/SKILL.md) 调研、整理引用、拟大纲或逐节修改长文。发送 `$content-research-writer 调研城市屋顶绿化，给我一份带来源链接的文章大纲`。查阅实时资料需要搜索和网页读取能力。

## 图表与网页

- [diagram-design](./diagram-design/SKILL.md) 制作轴测图、架构图、流程图等。发送 `$diagram-design 画一张山间图书馆轴测图，输出 HTML`。校验脚本需要 Python，PNG 导出还需要 Python Playwright 和对应的 Chromium。
- [moli-websearch](./moli-websearch/SKILL.md) 按关键词搜索网页或以图搜图。发送 `$moli-websearch 搜索 PowerShell 官方的执行策略文档，返回来源链接`。
- [moli-webfetch](./moli-webfetch/SKILL.md) 读取指定网页，也可生成截图。发送 `$moli-webfetch 读取 https://example.com 并总结页面内容`。
- [moli-cdp-server](./moli-cdp-server/SKILL.md) 启动本地 CDP 服务，供浏览器自动化客户端连接。发送 `$moli-cdp-server 启动本地 CDP 服务并检查连接端点`。

这三个 Moli Skill 都需要本机可运行 `moli`。可用 `moli --version` 检查。

## Codex 本地维护

- [keep-codex-fast](./keep-codex-fast/SKILL.md) 检查 Codex 会话、日志、工作树和配置。发送 `$keep-codex-fast 只读检查本地 Codex 状态，给我一份报告`。脚本需要 Python，默认只生成报告。
