---
name: model-switch
displayName: Model Switch
version: 1.0.0
description: 用自然语言指令切换和添加 AI 模型，支持智能判断模型特性和一键配置。
license: MIT-0
acceptLicenseTerms: true
tags: model, switch, multi-model, configuration
---

# Model Switch 技能

用自然语言指令切换和添加 AI 模型。

## 功能

### 切换模型
- `use <model>` - 切换到指定模型
- `切换模型` - 进入交互式引导
- `当前模型` - 查看当前模型

### 新增模型（优化版）
- `新增模型` - 进入优化后的新增流程
- 智能判断模型特性
- 一键配置 API Key
- 自动保存配置

## 使用

```bash
# 切换模型
python3 scripts/switch-model.py gemini

# 新增模型（优化版）
python3 scripts/add-model-guide.py

# 查看模型列表
python3 scripts/check-status.py
```

## 预置提供商

1. Google (Gemini)
2. OpenAI (GPT)
3. Anthropic (Claude)
4. Qwen (通义千问)
5. Moonshot (Kimi)
6. MiniMax
7. GLM (智谱)
8. DeepSeek
9. Custom Provider

## 优化特性

- ✅ 智能判断模型特性（图片/推理支持）
- ✅ 预置默认参数（contextWindow/maxTokens）
- ✅ 简化操作流程（一轮对话完成）
- ✅ 自动配置 API Key
- ✅ Endpoint compatibility 支持

---

## 🔒 安全说明

- **本地执行：** 所有脚本在本地运行，不联网
- **权限范围：** 仅需读取 ~/.openclaw/ 目录
- **无外部依赖：** 不克隆外部仓库，所有代码已包含
- **数据安全：** 不上传任何数据到外部服务器

---

**作者：** @williamwg2025  
**版本：** 1.0.1  
**许可证：** MIT-0
