# 超级IO（Super IO）白皮书

以大语言模型为核心数据总线的万物语义互联架构。

> 🌐 *English readers: [README.en.md](./README.en.md)*

## 📄 文档

| 文档 | 版本 | 说明 |
|------|------|------|
| [主文档：万物语义互联架构](./super-io-whitepaper.md) ([EN](./super-io-whitepaper.en.md)) | v0.2 | 通用架构定义（三层架构、语义中继、液态数据总线、终身学习环路），家居/割草机器人用例 |
| [工业分册：工厂人机协作安全系统](./super-io-whitepaper-industrial.md) ([EN](./super-io-whitepaper-industrial.en.md)) | v0.3 | 叉车/AGV/机械臂/PLC 的碰撞预判与安全语义融合，华东汽车零部件工厂用例 |
| [第二部分：扩展用例与技术深潜](./super-io-whitepaper-part2.md) ([EN](./super-io-whitepaper-part2.en.md)) | v0.2 | 扩展场景深入剖析 |
| [参考文献](./super-io-whitepaper-references.md) ([EN](./super-io-whitepaper-references.en.md)) | — | 21 篇学术论文与开源项目引用详情 |

## 🏗 文档结构

```
super-io-whitepaper/
├── README.md                              # ← 你在这里（中文）
├── README.en.md                           # English README
├── super-io-whitepaper.md                # 主文档（第1-8章 + 参考文献）
├── super-io-whitepaper.en.md             # English: Main document
├── super-io-whitepaper-industrial.md     # 工业场景分册
├── super-io-whitepaper-industrial.en.md  # English: Industrial supplement
├── super-io-whitepaper-part2.md          # 扩展用例
├── super-io-whitepaper-part2.en.md       # English: Extended use cases
├── super-io-whitepaper-references.md     # 参考文献调研笔记
└── super-io-whitepaper-references.en.md  # English: References
```

## 🔗 分册关联

主文档和分册通过 Markdown 相对路径超链接互相关联。主文档定义通用架构（Schema / LLM 引擎 / 三层设计），分册在通用架构基础上展开特定场景的用例验证。

## 📝 状态

- 主文档 v0.2：草案完成，待审核
- 工业分册 v0.3：草案完成，待审核

## 👥 贡献

Issues 和 PR 欢迎提交。分册写作请从 `master` checkout feature 分支，单独修改对应文件以避免冲突。
