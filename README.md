# Useful-SKILL

个人常用 Cursor / Claude Code Agent Skills 合集，方便安装与追溯出处。

## 包含的 Skills

| Skill | 作用 | 原出处 |
| --- | --- | --- |
| [`frontend-design`](skills/frontend-design/) | 高辨识度、非模板化的前端视觉设计 | [anthropics/claude-code](https://github.com/anthropics/claude-code/tree/main/plugins/frontend-design/skills/frontend-design) |
| [`grill-me`](skills/grill-me/) | 对计划/设计进行高压追问，达成共识后再动手 | 改编自 [mattpocock/skills](https://github.com/mattpocock/skills/tree/main/skills/productivity/grill-me) |
| [`check-prd-skill`](skills/check-prd-skill/) | 用 14 维度审查 B 端 PRD | [pmYangKun/check-prd-skill](https://github.com/pmYangKun/check-prd-skill) |
| [`create-prd-skill`](skills/create-prd-skill/) | 生成结构化 B 端 PRD | [pmYangKun/create-prd-skill](https://github.com/pmYangKun/create-prd-skill) |
| [`spec-plan`](skills/spec-plan/) | Spec 驱动开发：收敛需求并落盘 Spec | [JunhuaLiu1/awesome-skills](https://github.com/JunhuaLiu1/awesome-skills/tree/main/skills/spec-plan) |
| [`ui-ux-pro-max`](skills/ui-ux-pro-max/) | UI/UX 设计智能库（样式/配色/字体/UX 指南，可检索） | [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) |
| [`spec-kit`](skills/spec-kit/) | GitHub Spec-Driven Development 工具包（CLI + 需求/技术方案模板） | [github/spec-kit](https://github.com/github/spec-kit) |

## 在 Cursor 中使用

把需要的 skill 目录复制到项目或用户 skills 目录，例如：

```text
.cursor/skills/<skill-name>/
```

或：

```text
~/.cursor/skills/<skill-name>/
```

每个 skill 至少需要包含 `SKILL.md`。

> **例外：`spec-kit`** 不是单个 Skill 文件夹，而是完整工具包。请按目录内 [`COLLECTION_NOTE.md`](skills/spec-kit/COLLECTION_NOTE.md) / 上游 README 用 `uv` 安装 `specify-cli`，不要整目录拷进 `.cursor/skills/`。

## 许可说明

各 skill 保留其上游许可证与归属：

- `frontend-design`：见目录内 `LICENSE.txt`（Apache 2.0，源自 Anthropic）
- `check-prd-skill` / `create-prd-skill`：以原作者 pmYangKun 仓库为准
- `ui-ux-pro-max`：MIT（NextLevelBuilder），见目录内 `LICENSE`
- `spec-kit`：见目录内 `LICENSE`（上游 github/spec-kit）
- 其余 skill：保留原作者声明；本仓库仅作整理与备份
