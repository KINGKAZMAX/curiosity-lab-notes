# 机器人与具身交互

[返回学习总览](../README.md) · [12 周安排](../12-week-plan.md) · [学习记录模板](../templates/learning-record.md)

稳定 ID：`robotics` · 建立日期：2026-10-27 · 状态：候选方向；一次只激活一项工程或研究任务。

用原创虚构设备的本地状态模拟学习人类接管、反馈和故障说明；本轮上游仅作状态图和代理交互参考，不当作机器人硬件库。

## 第一步

写出机器人运行、暂停、人工接管、连接丢失四种模拟界面状态。

## 本次输出

一张模拟状态图、两个故障样例和一份预期反馈表。

## 验收条件

- [ ] 人工接管入口明确
- [ ] 连接丢失时不会把旧状态显示为最新
- [ ] 只声称模拟验证，不声称真实硬件或临床结果

## 本轮外部来源与个人 Fork

| 个人 Fork | 外部上游 | 学习与改造计划 |
|---|---|---|
| [KINGKAZMAX/excalidraw](https://github.com/KINGKAZMAX/excalidraw) | [excalidraw/excalidraw](https://github.com/excalidraw/excalidraw) | [专属计划](https://github.com/KINGKAZMAX/excalidraw/blob/master/KINGKAZMAX-STUDY.md) |
| [KINGKAZMAX/hermes-agent](https://github.com/KINGKAZMAX/hermes-agent) | [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) | [专属计划](https://github.com/KINGKAZMAX/hermes-agent/blob/main/KINGKAZMAX-STUDY.md) |

这些入口来自本轮检索的外部项目及其新建 Fork。练习采用原创的小场景；Fork 和学习计划本身不表示已经掌握工具，也不表示改动已被上游接受。

## 相关新学习笔记

- [visible human override in robot controls](../../notes/human-ai-interaction/visible-human-override-in-robot-controls.md)
- [uncertainty in rehabilitation prototype feedback](../../notes/human-ai-interaction/uncertainty-in-rehabilitation-prototype-feedback.md)
- [evidence logs for interaction experiments](../../notes/human-ai-interaction/evidence-logs-for-interaction-experiments.md)

## 从计划进入实际贡献

先完成一个小输出，再保存真实日期、修改理由和检查结果。文档可以标记为已起草；代码只有经过对应检查才标记为已验证。向上游提交的问题、PR 和最终合并状态分别记录，不把个人 Fork 的存在当作上游贡献。
