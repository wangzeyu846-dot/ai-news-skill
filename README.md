# AI 资讯快报

一个面向 Codex 的中文 Skill：说出「给我AI资讯」，搜集最近 72 小时的全球 AI 动态，核验与去重后，整理成便于阅读的飞书文档。

## 产品介绍网站

[查看「智能资讯助手」网站](https://wangzeyu846-dot.github.io/ai-news-skill/)

网站源码与发布文件位于本仓库的 [gh-pages 分支](https://github.com/wangzeyu846-dot/ai-news-skill/tree/gh-pages)，通过 GitHub Pages 免费托管。

## 内容与交付

- 覆盖模型与产品、技术与研究、行业与商业，兼顾国内外。
- 通常精选 8–10 条；符合标准的消息不足时少写，不凑数量。
- 每条包含事实摘要、关键数据或变化、使用条件与局限、通俗解读和原文链接。
- 飞书排版使用导航目录、分级标题、重点速览、加粗、列表和分割线。
- 每次新建文档，确认云端保存后返回链接；写入受阻时保留本地草稿。

## 安装

将本仓库中的 `ai-news` 文件夹复制到 `${CODEX_HOME:-$HOME/.codex}/skills/`，保持目录结构：

```text
skills/ai-news/
├── SKILL.md
├── agents/openai.yaml
└── references/
    ├── editorial.md
    └── feishu-delivery.md
```

在 Codex 重新加载技能后，用「给我AI资讯」或 `$ai-news` 调用。

## 运行条件

需要可用的联网搜索与网页读取能力。飞书交付需要支持文档写入的连接，或可操作的、已登录飞书的浏览器/客户端会话。Skill 本身不包含飞书 API 客户端、凭据或独立后台服务。

这是按需执行的技能，不会自动建立定时任务。用户可以在请求中覆盖时间范围、主题、篇幅和交付目录。飞书没有可用接入时，采集与本地草稿仍可完成。

## 文件说明

- [技能入口](ai-news/SKILL.md)：默认规格、采集筛选和交付流程。
- [信源与编辑标准](ai-news/references/editorial.md)：核验和内容质量规则。
- [飞书交付](ai-news/references/feishu-delivery.md)：接入、排版、保存验证与恢复。

## 贡献

欢迎通过 Issue 或 Pull Request 提出信源、内容密度、排版或接入改进。请不要提交账号凭据、私人文档地址或未经核验的示例新闻。

## 许可证

本项目的技能指令与文档采用 [MIT License](LICENSE)。引用的新闻、论文和第三方网站内容仍适用各自的版权与使用条款。
