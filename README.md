# openclaw-flomo-skill

轻量 flomo 风格笔记 Skill for OpenClaw。快速记录想法、搜索回顾。

## 功能

| 触发词 | 动作 |
|--------|------|
| 「记一下 xxx」「记笔记 xxx」 | 新增笔记 |
| 「搜笔记 xxx」 | 关键词搜索 |
| 「#标签 的笔记」 | 按标签筛选 |
| 「随机回顾」「随机一条笔记」 | 随机展示旧笔记 + AI 追问 |

## 数据文件

笔记存储在：`~/Documents/hub/areas/personal/memos.md`

格式：

```
## 2026-04-05 10:32
用户原文 #手动标签
AI标签：#自动标签1 #自动标签2

---
```

## 安装

将此 skill 放入 OpenClaw workspace 的 skills 目录：

```bash
git clone https://github.com/chester-zhou/openclaw-flomo-skill.git ~/.openclaw/workspace/skills/memo-notes
```

然后重启 OpenClaw。

## 与 Claude Code 共用数据

此 skill 与 [claude-memo](https://github.com/chester-zhou/claude-memo) 共用同一个数据文件，可在两个平台上无缝记录与检索。

## License

MIT
