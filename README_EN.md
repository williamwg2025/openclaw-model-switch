# Model Switch for OpenClaw

Switch AI models with natural language commands.

[中文版本](README_CN.md)

---

## ✨ Features

- 🔄 **Smart Switching** - "use gemini" or "切换到千问"
- 🆕 **Add New Models** - Support 9 pre-configured providers (Google, OpenAI, Anthropic, etc.)
- 🧠 **Auto-Detection** - Automatically detect image/reasoning support
- ⚙️ **One-Click Config** - Auto-save API Key and model configuration

---

## 🚀 Installation

```bash
cd /root/.openclaw/workspace/skills
git clone https://github.com/williamwg2025/openclaw-model-switch.git model-switch
chmod +x model-switch/scripts/*.py
```

---

## 📖 Usage

### Switch Models

```bash
# Switch to Gemini
python3 model-switch/scripts/switch-model.py gemini

# Switch to Claude
python3 model-switch/scripts/switch-model.py claude

# View current model
python3 model-switch/scripts/list.py
```

### Add New Models

```bash
python3 model-switch/scripts/add-model-guide.py
```

**Supported Providers:**
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

## 📋 Configuration

Model config saved at:
`/root/.openclaw/workspace/skills/model-switch/config/models.json`

---

## 🛠️ Scripts

| Script | Function |
|--------|----------|
| `switch-model.py` | Switch models |
| `add-model-guide.py` | Add model wizard |
| `list.py` | List models |
| `check-status.py` | Check status |

---

## 📄 License

MIT-0

---

**Author:** @williamwg2025  
**Version:** 1.0.0
