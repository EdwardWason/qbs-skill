# Changelog

## 1.0.0 (2026-09-19)

- 首个规范版本（v1.0.0），对齐 skill-forge 5 大撰写原则与 10 项发布前自检清单
- 重命名：名称「拷问书籍方法论」，slug `qbs-skill`，主触发词「拷问书籍方法论」
- **自依赖改造**（去除外部技能硬依赖）：
  - 找书漏斗内化七轴比对与四层降级链，本地书库工具不可用时直接走网络核验
  - 蒸馏协议内化 L1/L4/L5 三层提取 + V1/V2/V3 三重验证（原依赖外部拆解技能）
  - 合成合约内化 4+1 模块组装与全书级扩展路线（原依赖外部萃取技能）
- references 从 5 份合并为 3 份（grill-protocol / book-and-reading / distill-and-synthesize），问题规格书模板并入拷问协议
- SKILL.md 重构为标准 4+1 模块（何时触发/任务/输出格式/规则/示例/故障排除）
- 补齐工程文件：README 中英双语（含用户须知与关闭方式）/ CHANGELOG / LICENSE / plugin.json / .gitignore
- 已完成一次端到端实测（AI 协作发现→论文骨架，产出 paper-skeleton-forge 子 Skill，验收 5 条 4 过 1 部分通过）

## 0.1.0 (2026-09-19)

- 初版（内部代号 GBS）：六阶段流水线设计 + 5 份 references + 首次端到端实测
