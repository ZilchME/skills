# Skills

自定义技能仓库。每个子目录包含一个独立的 skill，通过 `SKILL.md` 文件注册。

## 技能列表

| Skill | 描述 |
|-------|------|
| [git-local-commit](git-local-commit/SKILL.md) | 根据对话上下文和 Git 改动，静默完成本地 commit（不 push） |

## 目录结构

```
skills/
├── README.md               ← 本文件，仅用于说明
├── git-local-commit/
│   └── SKILL.md             ← 技能定义（唯一被 Claude Code 加载的文件）
└── ...
```

## 添加新 Skill

1. 在根目录下创建子目录，如 `my-skill/`
2. 在子目录中创建 `SKILL.md`，遵循标准 frontmatter 格式
3. Skill 会被 Claude Code 自动识别并注册

> 注意：`README.md` 不会被 Claude Code 加载或解析，不影响技能注册和使用。
