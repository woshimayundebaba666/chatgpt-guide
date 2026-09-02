---
title: CCS 的使用注意事项
date: 2026-09-02 13:00:00
comments: false
---

这里说的 **CCS** 是指 **CC Switch**。它可以保存多套模型服务配置，并在 ChatGPT 官方登录与不同 API 服务之间进行切换。

## CCS 可以用来切换 API

当你需要测试不同服务商、使用自己的 API Key，或者临时切换 API 地址时，可以在 CC Switch 中选择对应的配置。切换后，Codex 会按照当前选中的服务方式连接模型。

不过对大多数普通用户来说，**没有必要专门切换到 API**。如果你已经拥有可以正常使用的 ChatGPT 套餐，直接选择图中的 **OpenAI Official**，使用自己的 ChatGPT 账号登录即可。

![在 CC Switch 中切换到 OpenAI Official，使用 ChatGPT 账号而不是 API](/ccs/images/cc-switch-openai-official.png)

{% success 大部分情况下这样选 open %}
点击上方的 OpenAI 图标，再选择 **OpenAI Official**。这种方式使用 ChatGPT 账号登录和套餐额度，不需要自行购买、填写或维护 API Key。
{% endsuccess %}

## 什么时候才需要 API

以下情况才有必要考虑 API：

- 你正在开发程序或自动化流程，需要让代码调用模型。
- 你明确知道 API 的服务地址、计费方式和数据处理规则。
- 你需要使用某个特定服务商提供的模型或功能。

OpenAI 官方说明中，ChatGPT 登录使用订阅访问权限；API Key 则按 API 用量单独计费，不会消耗 ChatGPT 套餐中包含的额度。因此，只是日常使用 Codex 时，通常无需切换。

{% warning API 安全提醒 open %}
API Key 相当于密码，可能产生实际费用。不要把它写进教程截图、聊天记录或公开文件，也不要使用来历不明的共享 Key。

第三方 API 的稳定性、价格、隐私政策和模型真实性由对应服务商负责。添加前请确认来源可信，并避免在不清楚规则的接口中处理敏感资料。
{% endwarning %}

## 切换后怎么确认

完成切换后重新打开 Codex，确认显示的是自己的 ChatGPT 账号，并尝试发送一条简单消息。如果能够正常响应，就不需要再修改其他配置。

## 官方资料

- [OpenAI：ChatGPT 登录与 API Key 登录的区别](https://learn.chatgpt.com/zh-Hans/docs/auth)
