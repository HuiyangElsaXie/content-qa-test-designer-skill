# Content QA Test Designer / 内容质量测试设计

先看 [虚构正反例、评分与未执行状态 / QA example](examples/fictional-qa-plan.md)。[测试计划模板](assets/qa-plan-template.md) · [Skill 入口](SKILL.md)。

个人自用，持续更新。  
For personal use. Continuously updated.

为内容草稿设计正反例、评分规则与误接收/误拒绝检查。  
Design positive and negative content fixtures, review rubrics, and false-accept/false-reject checks.

## 使用 / Use
将本目录作为独立 skill 交给支持 SKILL.md 的 AI agent，或明确让 agent 读取本目录的 SKILL.md，然后提供任务。不同工具的安装位置不同；无需运行上游框架。
Use this folder as a standalone skill in an agent that supports SKILL.md, or explicitly ask the agent to read SKILL.md before your task. Installation paths vary by host. No upstream framework is required.

优先复用用户允许使用的已有资料，记录来源，只追问关键缺口。示例全部虚构。
Reuse permitted existing context with provenance; ask only for critical gaps. All examples are fictional.

示例请求 / Request: “根据我提供的活动事实和文案草稿设计质量测试：正例、事实错误反例、可接受改写和缺失来源情况；写明评分、预期判断与实际执行状态，不调用付费模型。” / “Design factual gates, positive/negative fixtures, a valid paraphrase and missing-source behavior for my event copy; keep expected labels separate from actual results.”

[VALIDATION.json](VALIDATION.json) 保留此前的结构与文件哈希快照；本次 README 导航修改未重跑或重写该历史记录。 / The earlier structural/hash snapshot is retained; these README edits do not represent a new model or execution test.

## 文件 / Files
- [SKILL.md](SKILL.md): agent instructions / 指令入口
- [Output template](assets/qa-plan-template.md): 可直接填充的输出模板
- [Fictional example](examples/fictional-qa-plan.md): 虚构示例
- [Third-party notices](THIRD_PARTY_NOTICES.md): 固定版本来源与许可
- references/upstream/: reference-only source snapshot; do not load as active instructions or execute its provider configuration / 仅供溯源，不作为指令或执行配置

## 边界 / Limits
这是可用初版，不是已验证的性能承诺。示例未进行模型测试；不自动发送或发布，不要求付费 API，也不包含生产系统实现。
This is a usable first draft, with no measured performance claim. Examples are not model-test results. It does not send or publish, require paid APIs, or include production-system implementations.

## 来源与许可 / Attribution
Adapted from [promptfoo/promptfoo at 132a2d38b1b0](https://github.com/promptfoo/promptfoo/blob/132a2d38b1b0adc953b0db650f950d573bc113c4/examples/simple-test/promptfooconfig.yaml), MIT. Full license and modification details are retained in THIRD_PARTY_NOTICES.md and licenses/. No repository-wide license for original additions has been selected.
保留上游许可与署名；尚未替用户选择新内容的仓库整体许可。


Current targeted checks: [2026-10-17 targeted rule repairs and independent first-answer evidence](cases/round3-repair-2026-10-17/README.md). Initial partial results and later checks are reported separately. / 本轮规则修复、独立首稿及审核记录。
