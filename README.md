## 🔥 Overview

This repository contains:

✔️ **n8n Workflow Library** – ready-to-import automation templates  
✔️ **AI Cookbooks for VLM Run** – notebooks and examples showing how to use the VLM Run APIs in Python and n8n

VLM Run is a developer-friendly **Visual AI platform** that enables extraction, transformation, and generation from visual data (images, documents, videos) with structured JSON outputs and visual reasoning capabilities. :contentReference[oaicite:0]{index=0}

---

## 📦 What's Inside

### 📁 Repository Structure
n8n-workflows/

├── workflows

└── README.md


## 📚 n8n Workflow Library

The `workflows/` folder contains `.json` files that can be **imported directly** in an n8n instance:

1. Open n8n (self-hosted or cloud)
2. Go to **Workflows → Import**
3. Upload a workflow `.json`
4. Configure node credentials (API keys, tokens, etc.)

Typical integrations include:
- Google Drive  
- Custom Webhooks  
- OpenAI / VLM Run Visual AI  
- Slack / Notion / Sheets automations  


## 📄 Workflow Index

| **Workflow Name** | **Use Case** |
|-------------------|--------------|
| **AI Fashion Virtual Try-On with Image & Video Generation for Telegram, Discord & YouTube** | Perfect for virtual try-ons, AI fashion demos or content automation pipelines.|
| **Auto Meeting Summarizer with Google Drive, VLM Run to Sheets** | Summarize meeting notes from records. |
| **Face Redaction Using VLM Run Chat Completion** | Privacy-preservation by blurring face images in media.|
| **Generate UGC marketing videos for eCommerce with VLM Run , Open A** | Generate marketing videos for businesses. |
| **Image to Ghibli Art Using VLM Run with Discord, Telegram, Pushover** | Convert real image to ghibli style. |
| **Video Generation from First Frame and Last Frame using VLM Run** | Generates a smooth transition video between two input frames. |
| **Write a WordPress post with AI (starting from a few keywords)** | Generate wordpress post using AI. |

# ⚙️ Setup

### 1️⃣ Install n8n  
https://docs.n8n.io/installation

### 2️⃣ Import Workflows  
n8n → **Import** → upload JSON from `/workflows`

### 3️⃣ Configure API Keys  
Depending on workflow:

- VLM Run  
- Google Drive  
- OpenAI-style agents  
- Notion / Sheets / Slack  
- Webhooks  

---

# 🆘 Support & Resources

### 📖 Docs  
https://docs.vlm.run/

### 💬 Discord  
https://discord.gg/AMApC2UzVY

### 🐦 Twitter  
https://twitter.com/vlmrun

---

# ⭐ Contributing

Pull requests welcome! You can add:

- New n8n workflows  
- Image/AI pipelines  
- Integration templates  
- Cookbook notebooks  

