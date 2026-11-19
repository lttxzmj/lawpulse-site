# 法脉落地页

[法脉](https://lttxzmj.github.io/lawpulse-site/)（LawPulse）是一款面向中国执业律师的
本地优先桌面法律研究工具（macOS / Windows）：内置 1513 部法律、司法解释与
行政法规，共 56182 条，断网可全文检索；AI 合同审查与法库问答给出的每条依据
都会回本地法库校验，可点回原文。无账号，AI 采用自带密钥（BYOK）模式。

本仓库只放这个落地页，由 GitHub Pages 托管（main 分支根目录）。

## 页面

| 文件 | 说明 |
|---|---|
| `index.html` | 落地页，下载按钮与版本号由页面底部的 `RELEASE` 常量统一填充 |
| `privacy.html` | 隐私政策 |
| `terms.html` | 用户协议与免责声明 |
| `llms.txt` | 给 AI 检索用的事实清单，改价格与版本时要同步 |
| `robots.txt` / `sitemap.xml` | 抓取规则与站点地图 |

## 开源生态

- [chinese-law-corpus](https://gitee.com/chengzi_h/chinese-law-corpus)：
  1513 部法规逐条结构化语料（CC0），本站法规库的数据源；
- [chinese-law-skills](https://github.com/lttxzmj/chinese-law-skills)：
  给 AI agent 的中国法技能库（法条引用核验、合同审查、诉讼计算器等 13 个）；
- [chinese-law-mcp](https://github.com/lttxzmj/chinese-law-mcp)：
  同一语料的 MCP 服务器。

## 不要直接改这里

页面源文件在法脉主仓库的 `docs/` 目录，本仓库的内容由主仓库的
`npm run publish:site` 覆盖式同步。直接在这里提交的改动，下次发布就会被覆盖掉。

## 下载

安装包不放在本仓库，托管在对象存储：
[macOS（Apple Silicon）](https://lawpulse-data-1256098921.cos.ap-beijing.myqcloud.com/download/LawPulse-0.11.0-arm64.dmg)
／[Windows 64 位](https://lawpulse-data-1256098921.cos.ap-beijing.myqcloud.com/download/LawPulse-0.11.0-x64.exe)。
