# 可验证的个人英语学习系统

这是一个面向成年学习者的长期英语学习项目。它把英语学习当作一个可迭代系统：通过可理解输入、闭卷调用、真实输出、反馈、重写和间隔复测，把“看得懂”逐步转化为“能稳定使用”。

IELTS 只用于阶段校准和未来的考试迁移，不决定日常课程。

## 继续学习

1. 阅读[当前状态](records/current-state.md)，确认唯一待完成任务。
2. 打开状态文件指向的 `training/weekN/dayNN_*.md`。
3. 按课程格式提交实际答案、用时和完成范围。
4. 批改后更新每日记录、错误库、掌握清单和当前状态。

## 系统如何工作

```text
学习者背景与目标
        ↓
可理解输入 → 闭卷调用 → 短输出 → 反馈与重写
     ↑                              ↓
难度调整 ← 当前状态 ← 每日证据 ← 间隔复测
        ↓
每 7 个学习日周测；每 4 个完整学习周最多一次 IELTS 校准
```

学习进度按“已完成学习日”计算，不按连续自然日计算。训练文件是任务，不是完成证据；只有实际答案和记录才能改变学习状态。

## 项目导航

| 文档或目录 | 唯一职责 |
|---|---|
| [learning-plan.md](learning-plan.md) | 100 个学习日路线、每日结构和升级门槛 |
| [docs/recording-standard.md](docs/recording-standard.md) | 文件命名、记录字段、证据和掌握规则 |
| [docs/assessment-and-ielts.md](docs/assessment-and-ielts.md) | Day 30/60/100 验收与 IELTS 使用边界 |
| [records/learner-profile.md](records/learner-profile.md) | 稳定的学习背景、目标和约束 |
| [records/current-state.md](records/current-state.md) | 当前能力快照和唯一下一步 |
| [records/error-bank.md](records/error-bank.md) | 活跃错误与 `+1 / +3 / +7` 复习队列 |
| [records/mastery.md](records/mastery.md) | 已掌握、正在形成和证据不足的能力 |
| `records/daily/` | 每个已完成学习日的原子证据 |
| `records/weekly/` | 每 7 个已完成学习日的聚合复盘 |
| `records/assessments/` | 里程碑与正式阶段检测 |
| `training/` | 课程材料；存在不代表已经完成 |
| [AGENTS.md](AGENTS.md) | AI 私教的执行规则 |

完整文档索引见 [docs/README.md](docs/README.md)。

## 数据与公开仓库

- 记录必要的原句证据，但不写雇主、客户、内部项目名、账号或凭据。
- 工作文档示例必须去标识化，不提交受版权保护的完整教材、音频或答案册。
- 原始音频、临时文件和非学习产物默认由 `.gitignore` 排除；文字转写和学习结论可以提交。
- 这是个人学习仓库。若公开到 GitHub，提交前应再次检查历史记录中的隐私信息。

## GitHub 初始化

本目录已经初始化为本地 Git 仓库。首次发布时自行创建 GitHub 仓库，再添加远端并推送；仓库是否公开、名称和许可证由学习者决定。
