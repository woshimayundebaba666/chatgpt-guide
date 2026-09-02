---
title: 下载 ChatGPT 安装包
date: 2026-09-02 13:00:00
comments: false
---

Windows 上安装 ChatGPT，建议优先走 **OpenAI 官方下载流程**。在部分网络环境中，打开官网或完成下载前，需要先准备一个能够正常访问 OpenAI 官网的网络连接；请同时遵守所在地的法律法规和网络规定。

## 方案一：通过官方渠道安装（推荐）

### 1. 进入 OpenAI 官方下载页面

只从 OpenAI 官方页面或 Microsoft Store 获取安装程序，不要随意运行来历不明的“破解版”或修改版。

<div style="margin: 1.6rem 0; text-align: center;">
  <a href="https://chatgpt.com/download/" target="_blank" rel="noopener noreferrer" style="display:inline-block;padding:.9rem 1.5rem;border-radius:.45rem;background:#2a272d;color:#fff;font-weight:700;text-decoration:none;box-shadow:0 .35rem 1rem rgba(0,0,0,.18);">前往 OpenAI 官方下载页面 →</a>
</div>

### 2. 按安装提示进入 Microsoft Store

运行官方安装程序后，Windows 可能提示转入 Microsoft Store 或调用 Store 相关组件。按照页面提示依次点击“获取”“安装”或“打开”，等待安装结束即可，不需要自行寻找其他安装源。

### 3. 登录并开始使用

安装完成后打开 ChatGPT，使用自己的 ChatGPT 账号登录。Codex 需要账号和网络连接才能调用模型，它不是完全离线运行的本地模型。

{% success 最稳妥的选择 open %}
Microsoft Store 能正常使用时，请优先采用方案一。它能获得正版签名、自动更新和较完整的系统集成功能。
{% endsuccess %}

## 方案二：Microsoft Store 损坏时的临时备用

我当时安装时遇到过 Microsoft Store 损坏、无法正常完成安装的问题。为了先获得一个可以协助排查电脑问题的工具，我保留了一份 **老版本 Codex 备用文件包**。

{% warning 先看清楚再下载 open %}
这份“微软codex.zip”来自个人网盘分享，**不是 OpenAI 官方 ChatGPT 安装包，也不是标准 MSIX 安装器**。它属于已经解包的旧版 Codex 程序文件，能否直接运行取决于 Windows 版本、系统组件和安全策略；无法保证在每台电脑上都能“解压即用”，也不会自动获得最新版本。

如果 Windows、浏览器或安全软件提示文件异常，请停止运行并改用官方渠道。不要关闭系统安全功能来强行安装。
{% endwarning %}

### 使用备用包

1. 点击下方按钮，从百度网盘保存 `微软codex.zip`。
2. 提取码为 **6pde**。
3. 下载完成后先用 Windows 安全中心扫描压缩包。
4. 将压缩包完整解压到一个固定文件夹，不要只从压缩软件窗口里直接运行。
5. 尝试运行解压目录中的 `app/Codex.exe`，再按提示登录 ChatGPT 账号。

<div style="margin: 1.6rem 0; text-align: center;">
  <a href="https://pan.baidu.com/s/1unY8Of9VkfPaEreCL_8D9g?pwd=6pde" target="_blank" rel="noopener noreferrer" style="display:inline-block;padding:.9rem 1.5rem;border-radius:.45rem;background:#3143ff;color:#fff;font-weight:700;text-decoration:none;box-shadow:0 .35rem 1rem rgba(49,67,255,.28);">下载老版本 Codex 备用包 →</a>
  <div style="margin-top:.65rem;opacity:.78;">文件：微软codex.zip　提取码：6pde</div>
</div>

### 选择 GPT-5.5

如果这个版本能够正常登录，并且模型选择器中显示 **GPT-5.5**，可以按下图选择它。GPT-5.5 是否出现取决于账号权限、应用版本和当时的模型供应情况；看不到时不要强行修改程序，请以选择器中实际可用的模型为准。

![Codex 中的 GPT-5.5 模型提示](/download/images/gpt-5-5-model.png)

## 让 Codex 帮你修复 Microsoft Store

备用版能够正常运行后，可以把遇到的 Microsoft Store 报错截图发给 Codex，让它先诊断原因，再协助使用 Windows 官方工具修复 Store。涉及管理员权限、重置或重装前，应先让 Codex 解释影响并征得你的确认。

你可以直接这样问：

> 请检查我的 Microsoft Store 为什么无法打开或安装应用。优先使用 Windows 官方修复方法，每一步先告诉我作用；涉及管理员权限、重置或重装前先询问我。修复后，请协助我从 OpenAI 官网或 Microsoft Store 安装最新版正版 ChatGPT/Codex。

{% note 最终目标 %}
方案二只用于临时排障。Microsoft Store 修复后，请回到方案一安装最新版正版 ChatGPT/Codex，并删除不再需要的旧版备用文件。
{% endnote %}

## 官方资料

- [OpenAI：Windows 应用部署与官方 MSIX 说明](https://learn.chatgpt.com/docs/enterprise/windows-deployment)
- [OpenAI：Codex 模型说明](https://learn.chatgpt.com/zh-Hans/docs/models)
