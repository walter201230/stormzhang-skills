# stormzhang-skills

帅张（stormzhang）风格写作 AI Skill，基于 [Agent Skills](https://agentskills.io) 开放标准。

通过"蒸馏"帅张公众号文章、知识星球精华等大量真实内容，提炼出其写作风格、思维模式和价值观，让 AI 能够以帅张的风格撰写长文内容。

## 可用 Skills

| Skill | 描述 | 触发词 |
|-------|------|--------|
| [stormzhang-writer](./stormzhang-writer/) | 帅张风格长文写作 | 帅张风格、写文章、写长文、帮我写一篇 |

## 安装方式

### Claude Code

将 `stormzhang-writer` 文件夹复制到 Claude Code 的 skills 目录：

```bash
# 全局安装（所有项目可用）
cp -r stormzhang-writer ~/.claude/skills/

# 项目级安装（仅当前项目可用）
cp -r stormzhang-writer .claude/skills/
```

安装后重启 Claude Code 即可自动识别。

### 一键安装

你也可以直接告诉 Claude Code：

> 帮我安装这个 skill：https://github.com/你的用户名/stormzhang-skills

### OpenClaw

```bash
cp -r stormzhang-writer ~/.openclaw/skills/
```

## 使用方式

安装后，在 Claude Code 中直接说：

- "用帅张的风格写一篇关于 XXX 的文章"
- "帅张风格，帮我写一篇公众号文章"
- "以 stormzhang 的语气写一篇长文分享"

Skill 会自动触发，按照帅张的写作风格生成 1000 字以上的长文内容。

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

1. 收集帅张公众号 1300+ 篇文章、知识星球 23 万字精华内容
2. 通过 AI 分析提炼写作风格、标志性表达、文章结构模式
3. 整理为 SKILL.md 指令文件 + references 参考素材
4. 反复测试调优，确保输出风格的一致性

## 致谢

- 写作风格参考自公众号「stormzhang」及知识星球「帅张和他的朋友们」
- Skill 格式参考 [khazix-skills](https://github.com/KKKKhazix/khazix-skills)

## License

MIT
