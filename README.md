# Model Switch for OpenClaw

用自然语言指令切换和添加 AI 模型。

[English Version](README.md)

---

## ✨ 功能特性

- 🔄 **智能切换** - "use gemini" 或 "切换到千问"
- 🆕 **新增模型** - 支持 9 个预置提供商（Google, OpenAI, Anthropic 等）
- 🧠 **智能判断** - 自动判断模型是否支持图片/推理
- ⚙️ **一键配置** - 自动保存 API Key 和模型配置

---

## 🚀 安装

```bash
cd ~/.openclaw/workspace/skills
# 技能已安装在：~/.openclaw/workspace/skills/model-switch
chmod +x model-switch/scripts/*.py
```

---

## 📖 使用

### 切换模型

```bash
# 切换到 Gemini
python3 model-switch/scripts/switch-model.py gemini

# 切换到 Claude
python3 model-switch/scripts/switch-model.py claude

# 查看当前模型
python3 model-switch/scripts/list.py
```

### 新增模型

```bash
python3 model-switch/scripts/add-model-guide.py
```

**支持提供商：**
1. Google (Gemini)
2. OpenAI (GPT)
3. Anthropic (Claude)
4. Qwen (通义千问)
5. Moonshot (Kimi)
6. MiniMax
7. GLM (智谱)
8. DeepSeek
9. Custom Provider

---

## 📋 配置

模型配置保存在：
`~/.openclaw/workspace/skills/model-switch/config/models.json`

---

## 🛠️ 脚本说明

| 脚本 | 功能 |
|------|------|
| `switch-model.py` | 切换模型 |
| `add-model-guide.py` | 新增模型向导 |
| `list.py` | 查看模型列表 |
| `check-status.py` | 检查当前状态 |

---

## 📄 许可证

MIT-0

---

**作者：** @williamwg2025  
**版本：** 1.0.0

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
