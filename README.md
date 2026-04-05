# openclaw-flomo-skill

轻量 flomo 风格笔记 Skill for OpenClaw。快速记录想法、随机回顾，并通过微信 clawbot 推送。

![demo](demo.gif)

## 功能

| 触发词 | 动作 |
|--------|------|
| 「记一下 xxx」「记笔记 xxx」 | 新增笔记，自动补充 AI 标签 |
| 「搜笔记 xxx」 | 关键词搜索 |
| 「#标签 的笔记」 | 按标签筛选 |
| 「随机回顾」「随机一条笔记」 | 随机展示旧笔记 + AI 追问，推送至微信 clawbot |

## 随机回顾 × 微信 clawbot

触发「随机回顾」后，skill 会：

1. 从 7 天前的笔记中随机选 1 条
2. 生成 1 个 AI 开放性追问（引导深度思考）
3. **通过微信 clawbot 推送**，让回顾在你最自然的场景里出现

## 数据文件

笔记存储在本地 Markdown 文件（路径可自定义）：

```
## 2026-04-05 10:32
用户原文 #手动标签
AI标签：#自动标签1 #自动标签2

---
```

## 安装

```bash
git clone https://github.com/chester-zhou/openclaw-flomo-skill.git ~/.openclaw/workspace/skills/memo-notes
```

重启 OpenClaw 即可使用。

## 与 Claude Code 共用数据

此 skill 与 Claude Code 的 memo skill 共用同一数据文件，可在 OpenClaw 和 Claude Code 两端无缝记录与检索。

## License

MIT
