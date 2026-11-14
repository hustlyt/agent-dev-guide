# 深入学习 AI Agent 开发

学习路线 + 持续更新的资料库：官方教程、社区课程、工程文章、论文、视频和 AI 生成的教程。

**网站：** https://hustlyt.github.io/agent-dev-guide/ · [更新日志](https://hustlyt.github.io/agent-dev-guide/changelog.html) · [RSS](https://hustlyt.github.io/agent-dev-guide/feed.xml)

## 怎么更新

每周一 09:00（北京时间）由定时任务自动运行，流程和质量标准见 [UPDATE_PLAYBOOK.md](UPDATE_PLAYBOOK.md)：

1. `scripts/check.py`：刷新 GitHub Star 和最近提交时间，检查所有链接（连续两次失败才算失效）
2. `scripts/discover.py`：从 GitHub、23 个官方/社区 RSS 源、博客页、Hacker News、Reddit、arXiv 搜集候选
3. agent 补充网络搜索，打开原文按 10 分制评分，≥ 7 分才收录
4. `scripts/build.py`：校验数据并生成 `docs/`，推送后由 GitHub Pages 发布

只依赖 Python 3.11+ 标准库和 `gh` CLI。

## 目录

| 路径 | 内容 |
|---|---|
| `data/resources.json` | 资料库（唯一数据源） |
| `data/changelog.json` | 更新日志 |
| `data/reviewed.json` | 已审核过的 URL，避免重复审核 |
| `data/sources.json` | 搜集用的数据源和关键词 |
| `content/` | 教程正文、页头和样式 |
| `docs/` | 生成的网站（不要手改） |
