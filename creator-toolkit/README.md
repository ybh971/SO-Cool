# 🎬 Creator Toolkit — AI 内容创作助手

一个 Claude Code 技能包，帮内容创作者 **找选题** + **一键生成多平台文案**。

目前支持：**抖音** | **小红书** | **B站**

---

## 能做什么

```
你说："/topic-finder 美甲 找3个选题"
  ↓ AI 实时搜索热点，给你3-5个选题建议（带热度依据和角度）

你选一个："夏日果冻美甲合集"
  ↓

你说："/content-adapter 夏日果冻美甲合集"
  ↓ AI 自动生成抖音版、小红书版、B站版三种文案

你复制粘贴，发布 ✅
```

---

## 安装（1 分钟）

### 方式一：直接复制（推荐，零门槛）
1. 下载这个文件夹
2. 把 `skills/` 里的两个文件复制到你当前项目的 `.claude/skills/` 目录
3. 把 `templates/` 和 `config/` 也复制过去
4. 编辑 `config/source-config.md`，改成你自己的领域
5. 在 Claude Code 中输入 `/topic-finder` 试试

### 方式二：git clone
```bash
git clone https://github.com/<your-username>/creator-toolkit.git
cd creator-toolkit
# 然后将 skills/ 复制到你的 Claude Code 项目目录
```

---

## 使用示例

见 [examples/sample-workflow.md](examples/sample-workflow.md)

---

## 文件说明

| 文件 | 作用 | 你需要改吗 |
|------|------|-----------|
| `skills/topic-finder.md` | 选题发现 Skill | ❌ 不用 |
| `skills/content-adapter.md` | 多平台适配 Skill | ❌ 不用 |
| `templates/douyin.md` | 抖音文案格式规范 | 可选（调风格） |
| `templates/xiaohongshu.md` | 小红书格式规范 | 可选（调风格） |
| `templates/bilibili.md` | B站格式规范 | 可选（调风格） |
| `config/source-config.md` | 你的领域和偏好 | ✅ 必须改 |
| `examples/sample-workflow.md` | 完整使用流程示例 | ❌ 不用 |

---

## 常见问题

**Q: 需要 API Key 吗？**
A: 不需要。完全依赖 Claude Code 内置的 WebSearch 和 Skill 工具。

**Q: 选题数据是实时的吗？**
A: 是。每次运行 topic-finder 都会实时搜索引擎结果，不是模型训练数据。

**Q: 能支持更多平台吗？**
A: 你可以自己在 `templates/` 里加新平台的格式规范，content-adapter 会自动读取。

**Q: 能给企业/团队用吗？**
A: MIT License，随便用。

---

## 后续计划

- [ ] 支持微信公众号格式
- [ ] 选题历史记录
- [ ] Web 版 SaaS（订阅制）

MIT License
