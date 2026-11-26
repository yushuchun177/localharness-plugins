# localharness-plugins

Local-Harness 的插件索引（6 个）。

主程序「设置 → 插件管理」读取 `index.json`，从各插件自己的仓库下载 zip 并部署到 `user://plugins/<id>/`。

| 插件 | 仓库 | 说明 |
| --- | --- | --- |
| 操作电脑 / Computer control | [yushuchun177/localharness-plugin-control](https://github.com/yushuchun177/localharness-plugin-control) | 移动鼠标、点击、输入文字、按键、列出并切换窗口。危险：会给模型操作桌面的能力。 |
| 上下文洞察 / Context insights | [yushuchun177/localharness-plugin-insights](https://github.com/yushuchun177/localharness-plugin-insights) | 看一眼当前对话有多大：消息数、字数、估算 token、还能塞多少；以及把早期历史压成摘要。 |
| 记忆系统 / Memory | [yushuchun177/localharness-plugin-memory](https://github.com/yushuchun177/localharness-plugin-memory) | 长期记忆：把用户偏好、事实记下来，需要时按关键词检索。存在本地 user:// 里，不上传。 |
| 截图 / Screenshot | [yushuchun177/localharness-plugin-screenshot](https://github.com/yushuchun177/localharness-plugin-screenshot) | 抓一张全屏截图存成 PNG，返回路径和分辨率（配合识图插件可以看图）。 |
| 终端 / Terminal | [yushuchun177/localharness-plugin-terminal](https://github.com/yushuchun177/localharness-plugin-terminal) | 在 Windows 上执行命令，把标准输出和退出码返回给模型。带危险命令黑名单。 |
| 网页搜索与获取 / Web search & fetch | [yushuchun177/localharness-plugin-web](https://github.com/yushuchun177/localharness-plugin-web) | 抓取网页正文（curl 转纯文本）和 DuckDuckGo 关键词搜索，把结果喂给模型。 |
