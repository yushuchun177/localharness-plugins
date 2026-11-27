# localharness-plugins

Local-Harness 的插件索引（13 个）。

主程序「设置 → 插件管理」读取 `index.json`，从各插件自己的仓库下载 zip 并部署到 `user://plugins/<id>/`。

| 插件 | 仓库 | 说明 |
| --- | --- | --- |
| 自动化任务 / Automation | [yushuchun177/localharness-plugin-automation](https://github.com/yushuchun177/localharness-plugin-automation) | 定时/延时跑一句话任务，结果写进「自动化」会话。程序开着的时候生效。 |
| 智能压缩上下文 / Smart compaction | [yushuchun177/localharness-plugin-compact](https://github.com/yushuchun177/localharness-plugin-compact) | 把较早的对话压成一条摘要，腾出上下文空间；摘要由模型自己写，插件负责安全地改历史。 |
| 操作电脑 / Computer control | [yushuchun177/localharness-plugin-control](https://github.com/yushuchun177/localharness-plugin-control) | 移动鼠标、点击、输入文字、按键、列出并切换窗口。危险：会给模型操作桌面的能力。 |
| 上下文洞察 / Context insights | [yushuchun177/localharness-plugin-insights](https://github.com/yushuchun177/localharness-plugin-insights) | 看一眼当前对话有多大：消息数、字数、估算 token、还能塞多少；以及把早期历史压成摘要。 |
| 记忆系统 / Memory | [yushuchun177/localharness-plugin-memory](https://github.com/yushuchun177/localharness-plugin-memory) | 长期记忆：把用户偏好、事实记下来，需要时按关键词检索。存在本地 user:// 里，不上传。 |
| OAR 智能体 / OAR agent | [yushuchun177/localharness-plugin-oar](https://github.com/yushuchun177/localharness-plugin-oar) | 把任务交给本机装的外部智能体命令行（codex / claude / ollama / llm…），拿回它的输出。 |
| 远程操作 / Remote | [yushuchun177/localharness-plugin-remote](https://github.com/yushuchun177/localharness-plugin-remote) | 把本机变成一个任务端点（HTTP），或者把任务发给另一台开着 Local-Harness 的机器。 |
| 截图 / Screenshot | [yushuchun177/localharness-plugin-screenshot](https://github.com/yushuchun177/localharness-plugin-screenshot) | 抓一张全屏截图存成 PNG，返回路径和分辨率（配合识图插件可以看图）。 |
| 子智能体 / Sub-agent | [yushuchun177/localharness-plugin-subagent](https://github.com/yushuchun177/localharness-plugin-subagent) | 另起一个独立的模型实例，带着自己的系统提示去处理子任务，只把结果交回来。 |
| 终端 / Terminal | [yushuchun177/localharness-plugin-terminal](https://github.com/yushuchun177/localharness-plugin-terminal) | 在 Windows 上执行命令，把标准输出和退出码返回给模型。带危险命令黑名单。 |
| 识图 / Vision / OCR | [yushuchun177/localharness-plugin-vision](https://github.com/yushuchun177/localharness-plugin-vision) | 看图：读取图片信息、用系统 OCR 提取文字；如果配了视觉模型（GGUF + mmproj）就直接描述画面。 |
| 语音输入 / Voice | [yushuchun177/localharness-plugin-voice](https://github.com/yushuchun177/localharness-plugin-voice) | 朗读回答（Windows 中文语音）；也能录一段麦克风并尝试用系统语音识别转成文字。 |
| 网页搜索与获取 / Web search & fetch | [yushuchun177/localharness-plugin-web](https://github.com/yushuchun177/localharness-plugin-web) | 抓取网页正文（curl 转纯文本）和 DuckDuckGo 关键词搜索，把结果喂给模型。 |
