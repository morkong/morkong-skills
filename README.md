# morkong-skills

个人 Claude Code 技能合集仓库，持续扩充中。

## 安装

```bash
# 添加个人插件源
/plugin marketplace add morkong-skills https://github.com/morkong/morkong-skills

# 安装
/plugin install morkong-skills@morkong-skills
```

## 技能列表

| 技能 | 触发方式 | 说明 |
|------|---------|------|
| `resource-collector` | 自动（匹配任务上下文） | 全网搜索学习资源 → 验证链接 → 整理为结构化 Markdown 表格 |

### resource-collector

当你说"帮我搜集 XX 考试的教程资源"、"整理 XX 的学习资料"等时自动激活。

**执行流程**：多维度搜索 → 补充收网 → 链接验证 → 结构化表格 → 输出备考建议。

**输出**：一份分类整理的 Markdown 资源大全文件，字段包括标题/描述/链接/推荐值/是否付费/学习进度。

## 如何添加新技能

1. 在 `skills/` 下新建目录，如 `skills/my-new-skill/`
2. 创建 `SKILL.md`，按规范编写 frontmatter 和内容
3. 提交 PR 或直接 push

```
skills/
├── resource-collector/
│   └── SKILL.md
└── my-new-skill/          ← 按此模板新增
    └── SKILL.md
```

## 许可

Apache-2.0
