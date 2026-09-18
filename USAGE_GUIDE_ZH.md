# 使用说明

这个 skill 的名字是：

`my-ai-automation-interview-coach`

它适合你准备这些岗位：

- AI Automation Developer
- AI Engineer
- Power Platform Developer
- RAG / LLM Application Developer
- Workflow Automation Engineer
- Full-stack AI Developer
- Microsoft AI / Automation Consultant

## 怎么调用

在 Codex / ChatGPT 里，你可以这样说：

```text
使用 my-ai-automation-interview-coach，给我做一轮 RAG system design mock，目标岗位是 AI Engineer，用英语问我。
```

或者：

```text
使用 my-ai-automation-interview-coach，深挖我的 FlowPilot AI 项目，不要帮我补答案，只追问。
```

也可以：

```text
使用 my-ai-automation-interview-coach，帮我分析这个 JD 和我的简历匹配度。
```

## 推荐练习方式

### 1. 项目深挖

最重要，优先练。

```text
使用 my-ai-automation-interview-coach，按 project-deep-dive-ladders 深挖 FlowPilot AI。每次只问一个问题，我答完再追问。
```

适合练：

- FlowPilot AI
- Gote Note
- Akavia RAG FAQ Assistant
- Akavia onboarding workflow
- Insutex Copilot / SharePoint
- SAS OpenAI + Rasa 项目
- CAN IDS thesis

### 2. 严格 mock

```text
使用 my-ai-automation-interview-coach，给我做严格 mock。按 calibration-rules 评分，默认从 2 分开始，不要鼓励式反馈。
```

这会避免模型一直说“不错，可以再补充一点”。

### 3. RAG / LLM 系统设计

```text
使用 my-ai-automation-interview-coach，模拟 45 分钟 RAG/LLM system design 面试。题目：设计一个内部 IT FAQ assistant。
```

重点会练：

- chunking
- embeddings
- retrieval
- citations
- fallback
- evaluation
- permissions
- prompt injection
- cost / latency

### 4. Power Platform 面试

```text
使用 my-ai-automation-interview-coach，问我 Power Platform Developer 面试题，重点是 Power Apps、Dataverse、Power Automate、Copilot Studio。
```

### 5. 瑞典市场面试

```text
使用 my-ai-automation-interview-coach，按 Sweden market interview 模块，帮我准备 Stockholm consulting company 的面试。
```

适合准备：

- HR screen
- consulting 客户面
- culture fit
- salary expectation
- work permit / local market questions

### 6. 英语表达训练

```text
使用 my-ai-automation-interview-coach，我用英语回答。请分开评价：内容分数、英语表达、术语是否自然。
```

### 7. 中英混合训练

```text
使用 my-ai-automation-interview-coach，解释和反馈用中文，但让我用英文回答面试题。
```

这个模式很适合你：中文理解策略，英文练真实表达。

### 8. Take-home 作业

```text
使用 my-ai-automation-interview-coach，帮我规划一个 4 小时 take-home assignment，题目是构建一个简单 RAG assistant。
```

它会帮你规划：

- scope
- 时间分配
- README
- tradeoffs
- TODO
- demo 讲法

### 9. 15 分钟项目 walkthrough

```text
使用 my-ai-automation-interview-coach，帮我练 15 分钟 FlowPilot AI project walkthrough。
```

结构是：

1. problem and users
2. architecture
3. key decisions
4. hardest tradeoff
5. security/reliability
6. demo/outcome
7. improvements

### 10. 弱点日志

```text
使用 my-ai-automation-interview-coach，结束本轮 mock，并按 weakness-log 输出 scorecard。下次 mock 开始前先读上一次扣分点。
```

日志实际写入：

```text
logs/YYYY-MM-DD_模块_主题.md
```

每次 mock 后记录：

- 日期
- 模块
- 维度分数
- 三个具体扣分点
- 下次重点
- 可复用追问

### 11. 反向提问

```text
使用 my-ai-automation-interview-coach，帮我准备问 hiring manager / future teammate / HR 的反向问题。
```

### 12. Offer / 薪资

```text
使用 my-ai-automation-interview-coach，按 Sweden offer negotiation 帮我分析这个 offer。不要编市场价，先问我具体 package。
```

### 13. 规则重校准

```text
/recalibrate
```

长 mock 中如果感觉反馈变松、开始安慰你、或者开始替你补答案，就发这个指令，让教练重新拉回严格规则。

## 最推荐你的训练顺序

1. FlowPilot AI 深挖
2. Gote Note 深挖
3. Akavia RAG FAQ Assistant 深挖
4. RAG system design mock
5. Power Platform case mock
6. Behavioral: career switch story
7. Sweden HR / culture fit
8. Coding/debugging: idempotency, auth filter, retry
9. Take-home strategy
10. 英语表达 mock

## 最有用的命令模板

```text
严格点，不要安慰我。按 1-4 分打分，默认 2 分，只有我说出具体证据才升分。
```

```text
不要帮我补答案。只指出缺什么，然后让我重新答。
```

```text
每次只问一个问题，像真实面试一样追问三层。
```

```text
我先用英文回答，你用中文指出内容问题，再给我一个更自然的英文版本。
```

```text
这个答案按瑞典面试风格会不会太自夸？帮我改得更自然。
```

```text
这轮结束后生成 scorecard，并把下次练习重点写出来。
```

```text
开始 live coding simulation。你模拟共享编辑器面试官，我边想边写，你不要直接给答案。
```
