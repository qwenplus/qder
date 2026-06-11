# Ollama API 模型可用性测试结果

测试时间：2024年
API Endpoint: https://api.ollama.com/api/tags

## 测试总结

- **总模型数**: 41 个
- **免费可用**: 27 个
- **需要订阅**: 14 个

---

## ✅ 免费可用模型 (27 个)

| 模型名称 | 大小 | 类型/备注 |
|---------|------|----------|
| **ministral-3:3b** | 4.67 GB | 轻量级模型，响应最快 |
| **gemma3:4b** | 8.6 GB | 轻量级模型，平衡性能与速度 |
| **gemma3:12b** | 24 GB | 中型模型 |
| **rnj-1:8b** | 16 GB | 中型模型 |
| **ministral-3:8b** | 10.4 GB | 中型模型 |
| **devstral-small-2:24b** | 51.6 GB | 中型模型 |
| **gemma3:27b** | 55 GB | 中型模型 |
| **nemotron-3-nano:30b** | 32.6 GB | 中型模型 |
| **gemma4:31b** | 62.5 GB | 中型模型 |
| **gpt-oss:20b** | 13.78 GB | 中型模型，通用任务 |
| **gpt-oss:120b** | 65.3 GB | 大型模型 |
| **ministral-3:14b** | 15.7 GB | 中型模型 |
| **qwen3-next:80b** | 81.8 GB | 大型模型 |
| **qwen3-coder-next** | 81.8 GB | 代码专用模型 |
| **devstral-2:123b** | 128.2 GB | 大型模型 |
| **minimax-m2** | 230 GB | 大型模型 |
| **minimax-m2.1** | 230 GB | 大型模型 |
| **minimax-m2.5** | 230 GB | 大型模型 |
| **nemotron-3-super** | 230.5 GB | 大型模型 |
| **minimax-m3** | 未知 | 最新模型 |
| **nemotron-3-ultra** | 未知 | 超大型模型 |
| **qwen3-vl:235b** | 470 GB | 视觉语言模型 |
| **qwen3-vl:235b-instruct** | 470 GB | 视觉语言指令模型 |
| **qwen3-coder:480b** | 510 GB | ⭐ 代码专用大模型 |
| **glm-4.6** | 696 GB | ⭐ 综合能力强，推荐 |
| **glm-4.7** | 696 GB | ⭐ 综合能力强，推荐 |
| **cogito-2.1:671b** | 688.6 GB | ⭐ 复杂推理任务 |

---

## ❌ 需要订阅的模型 (14 个)

| 模型名称 | 大小 |
|---------|------|
| qwen3.5:397b | 397 GB |
| deepseek-v4-flash | 140 GB |
| gemini-3-flash-preview | 未知 |
| glm-5 | 756 GB |
| mistral-large-3:675b | 682 GB |
| deepseek-v4-pro | 1.6 TB |
| deepseek-v3.1:671b | 688.6 GB |
| kimi-k2-thinking | 1.12 TB |
| kimi-k2.6 | 595 GB |
| deepseek-v3.2 | 688.6 GB |
| glm-5.1 | 1.51 TB |
| kimi-k2:1t | 1.12 TB |
| kimi-k2.5 | 1.12 TB |
| minimax-m2.7 | 480.8 GB |

---

## 💡 推荐使用策略

### 免费大模型首选
- **glm-4.7** / **glm-4.6** - 综合能力最强，适合通用任务
- **qwen3-coder:480b** - 编程和代码相关任务
- **cogito-2.1:671b** - 复杂推理和逻辑任务
- **qwen3-vl:235b** - 图像理解和多模态任务

### 轻量快速模型
- **ministral-3:3b** - 最快响应，适合简单任务
- **gemma3:4b** - 性能与速度的最佳平衡
- **gpt-oss:20b** - 通用日常任务

---

## 测试方法

使用以下 PowerShell 命令获取模型列表：
```powershell
Invoke-RestMethod -Uri "https://api.ollama.com/api/tags" -Headers @{Authorization="Bearer <YOUR_API_KEY>"}
```

逐个测试模型可用性，返回成功即为免费可用，返回 "this model requires a subscription" 则需要付费订阅。

---

*最后更新：2024年*
