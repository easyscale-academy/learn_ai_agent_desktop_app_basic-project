---
description: "你已经在 Codex Desktop 里添加了本教学仓库作为 project, 照着二十四张截图把每个操作走了一遍, 让 AI 根据截图写出一份文档, 用 summarize skill 生成了一份摘要, 并成功 fork 出一个只继承部分历史的新对话."
---

# 走通 Codex Desktop 的完整操作

## 1. 目标

把 Codex 桌面版从添加项目到用上 Agent Skill 的整条路径亲手走一遍. 目标不是记住每个按钮的名字, 而是让这个 App 从 "满屏不认识的东西" 变成 "我知道每个地方是干嘛的".

走完之后你手上会留下两份真实产出, 都在你自己的 repo 里: 一份 AI 根据截图写出来的说明文档, 一份 Agent Skill 生成的长文摘要.

---

## 2. 要做的事情

1. 把这个教学仓库 clone 到本地. 打开 ChatGPT 桌面客户端, 左上角从 ChatGPT 切换到 Codex.
2. 用 New project 把 clone 下来的文件夹添加成一个 project, 发出第一条消息确认链路是通的.
3. 把 Local, main, 审批模式, Model, Effort, Speed 这六个 widget 挨个点开看一遍, 把审批模式设成 Approve for me.
4. 把 Codex 界面本身截个图粘进输入框, 让它根据这张图写一份文档到 tmp 目录下的某个 md 文件里. 写完点 Review 看 diff, 再用右侧加号打开 Files 在文件浏览器里看一眼渲染效果.
5. 读它写的这份文档, 挑一处跟你实际看到的界面对不上的地方, 再截一张图追问, 并让它联网搜一下, 看它怎么修正自己.
6. 在文件树里找到 resources 目录下的 openai-agent-skills.md, 右键 Add to chat. 输入斜杠加 summari, 按 Tab 补全, 后面接 this file 发送, 观察输出的结构.
7. 输入斜杠加 status, 看一眼上下文剩余和额度剩余, 并想清楚这个数字为什么比你的直觉大.
8. 挑中间任意一条消息点 fork, 选 Use this workspace, 确认新对话只继承到那条消息为止.

**预计用时:** 90 到 120 分钟

---

## 3. 检查清单

- [ ] **项目已添加**: 你在 Codex 里创建了 project, 中间的大字变成了 What should we build in 加上你的项目名, 并且第一条消息成功收到了回复.
- [ ] **认识每个 widget**: Local, main, 审批模式, Model, Effort, Speed 六个你都点开看过, 并且能说出各自是干什么的.
- [ ] **审批模式的取舍**: 你能说清 Approve for me 为什么是日常首选, 以及 Full access 为什么只适合能为自己损失兜底的人.
- [ ] **Effort 的判断**: 你能举出至少两种任务, 分别说明该用低档还是高档, 并说清为什么不是越高越好.
- [ ] **交材料与写文件**: 你用截图交过材料, 也让 AI 把产出写到了你指定的路径, 并且知道 tmp 目录是被 gitignore 的临时区.
- [ ] **截图问 AI 这个方法**: 你把界面截图丢给 AI 问过一次, 也针对一处对不上的地方追问过一次并让它联网搜, 并且认可这是搞懂任何陌生软件最直白的一条路.
- [ ] **审阅改动**: 你点过 Review 看 diff, 也用文件浏览器打开过生成的文件.
- [ ] **用过 Agent Skill**: 你成功召唤了 summarize skill 并拿到了摘要, 并且能指出这个 skill 的真身就是 .agents 目录下 summarize 里的那个 SKILL.md 文件.
- [ ] **理解上下文**: 你用 status 看过上下文和额度, 能说出至少三样占着上下文但在聊天记录里看不见的东西 (读过的文件全文, 中间步骤, 被召唤的 SKILL.md, 它写出去的内容), 并能讲清为什么重要结论要写进文件而不是留在对话里.
- [ ] **fork 成功**: 你 fork 出了一个新对话, 并确认它只继承了到 fork 那条消息为止的历史.
