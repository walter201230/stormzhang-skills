# stormzhang-skills

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

stormzhang 风格写作 AI Skill，基于 [Agent Skills](https://agentskills.io) 开放标准。

通过"蒸馏" stormzhang 公众号 1300+ 篇文章、知识星球 23 万字精华内容，提炼出其写作风格、思维模式和价值观，让 AI 能够以 stormzhang 的风格撰写长文内容。

## 可用 Skills

| Skill | 描述 | 触发词 |
|-------|------|--------|
| [stormzhang-writer](./stormzhang-writer/) | stormzhang 风格长文写作 | stormzhang 风格、写文章、写长文、帮我写一篇 |

## 安装方式

### 方式一：手动安装

```bash
# 克隆仓库
git clone https://github.com/walter201230/stormzhang-skills.git

# 全局安装（所有项目可用）
cp -r stormzhang-skills/stormzhang-writer ~/.claude/skills/

# 或项目级安装（仅当前项目可用）
cp -r stormzhang-skills/stormzhang-writer .claude/skills/
```

安装后重启 Claude Code 即可自动识别。

### 方式二：一键安装

在 Claude Code 中直接说：

> 帮我安装这个 skill：https://github.com/walter201230/stormzhang-skills

### 其他平台

```bash
# OpenClaw
cp -r stormzhang-writer ~/.openclaw/skills/

# Codex
cp -r stormzhang-writer ~/.agents/skills/
```

## 使用方式

安装后，在 Claude Code 中直接说：

- "用 stormzhang 的风格写一篇关于 XXX 的文章"
- "stormzhang 风格，帮我写一篇公众号文章"
- "以 stormzhang 的语气写一篇长文分享"

Skill 会自动触发，按照 stormzhang 的写作风格生成 1000 字以上的长文内容。

## 风格特点

- **白话文为主**：像跟朋友聊天，不追求华丽辞藻
- **真实经历驱动**：用个人经历和身边案例作为论据
- **观点鲜明直接**：敢说，不绕弯子
- **接地气的案例**：烧饼摊、发传单、闲鱼，而不是高大上的商业理论
- **反鸡汤**：不说正确的废话，给具体可操作的建议

## 文件结构

```
stormzhang-writer/
├── SKILL.md                      # 核心指令文件
└── references/
    ├── style_examples.md          # 风格范例集（原文摘录）
    └── content_methodology.md     # 内容方法论（选题、读者画像）
```

## 什么是"蒸馏 Skill"？

"蒸馏 Skill"是一种通过收集一个人的大量内容素材（文章、演讲、视频等），提炼出其写作风格、思维模式和价值观，封装成 AI 可用的技能包的方法。

本项目的制作流程：

1. 收集 stormzhang 公众号 1300+ 篇文章、知识星球 23 万字精华内容
2. 通过 AI 分析提炼写作风格、标志性表达、文章结构模式
3. 整理为 SKILL.md 指令文件 + references 参考素材
4. 反复测试调优，确保输出风格的一致性

## 致谢

- 写作风格参考自公众号「stormzhang」及知识星球「stormzhang 和他的朋友们」
- Skill 格式参考 [khazix-skills](https://github.com/KKKKhazix/khazix-skills)

## License

MIT
