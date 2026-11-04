# Drama Skills · short-drama

> **[short-drama](https://github.com/simlpandordinary/short-drama)** —— 飞书《WorkBuddy 视频系列 · 全技能与提示词总目录》里推荐的开源技能，已拆分为独立仓库分发（一个技能一个仓库）。

| 项 | 内容 |
| - | - |
| 上游仓库 | <https://github.com/zenstory-ai/drama-skills> |
| 上游路径 | `skills/short-drama` |
| 上游协议 | MIT |
| 上游 Star | 3.7k+ |
| 拆分方式 | 仅抽取该技能自身文件，独立可用 |

## 技能说明

基于文件系统初始化和继续短剧或漫剧项目，提供 creator-first 五文档路由、本地 Dashboard、制作形态与 Look Development 决策。用户提出“创建/继续短剧项目”“看进度/下一步”“做 Look Development”“打开 dashboard/短剧创作台”“导出制作资料”，或任务跨多个创作阶段时使用；明确的写作、资产、提示词、分镜、剪辑或审查请求由对应子 skill 直接处理。

## 目录结构

```
├── LICENSE
├── README.upstream.md
├── SKILL.md
├── scripts/
├── creator_markdown_check.py
├── creator_views.py
├── dashboard_server.py
├── project_tool.py
└── selftest.py
├── references/
├── audience-reveal.md
├── contract-and-ownership.md
├── creator-documents.md
├── creator-workflow.md
├── knowhow-index.md
├── look-development.md
├── pickup-and-alternate.md
├── production-form-profiles.md
├── reference-roles.md
├── runtime-preflight.md
└── form-cards/
├── Q版表达.md
├── 二维动态漫.md
├── 国漫二次元.md
├── 实拍.md
├── 水墨笔触.md
└── 风格化三维.md
├── assets/
├── creator-decision.example.jsonl
├── production-observation.example.jsonl
├── reference-observation.example.jsonl
├── project-template/
└── short-drama.json
└── dashboard/
├── app.js
├── index.html
├── styles.css
└── tokens.css
└── agents/
└── openai.yaml
```

- `SKILL.md` 是技能入口（触发条件 / 工作流 / 约束），安装时必须位于技能根目录。
- `references/`、`scripts/`、`assets/` 为该技能自带的参考文档、脚本与素材。
- `README.upstream.md` 为上游仓库原始说明，保留出处与版权信息。
- `LICENSE` 为上游许可证原件。

## 安装

WorkBuddy 技能目录为 `~/.workbuddy/skills/short-drama/`：

```bash
git clone https://github.com/simlpandordinary/short-drama.git ~/.workbuddy/skills/short-drama
```

也可以直接对 AI 说：「把 <https://github.com/simlpandordinary/short-drama> 装成 Skill」。

安装后用自然语言触发，例如「Drama Skills · short-drama」「用 short-drama 帮我处理这个任务」。

## 版权

原始作者与版权归上游仓库 `zenstory-ai/drama-skills` 所有。本仓库仅做独立分发与结构整理，未修改技能内容；商用请遵循上游许可证。
