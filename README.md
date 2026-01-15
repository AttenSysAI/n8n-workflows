<div align="center">
  <img src="https://raw.githubusercontent.com/vlm-run/.github/refs/heads/main/profile/assets/vlm-black.svg" alt="VLM Run Logo" width="80" />
  <h1 align="center">VLM Run AI Cookbooks + n8n Workflows</h1>
  <p align="center">
    <a href="https://vlm.run"><strong>Website</strong></a> |
    <a href="https://app.vlm.run/"><strong>Platform</strong></a> |
    <a href="https://github.com/vlm-run/vlmrun-hub"><strong>VLM Run Hub</strong></a> |
    <a href="https://docs.vlm.run/"><strong>Docs</strong></a> |
    <a href="https://vlm.run/blog"><strong>Blog</strong></a> |
    <a href="https://discord.gg/AMApC2UzVY"><strong>Discord</strong></a>
  </p>
  <p align="center">
    <a href="https://discord.gg/AMApC2UzVY"><img alt="Discord" src="https://img.shields.io/badge/discord-chat-purple?logo=discord"></a>
    <a href="https://twitter.com/vlmrun"><img alt="Twitter Follow" src="https://img.shields.io/twitter/follow/vlmrun.svg?style=social&logo=twitter"></a>
  </p>
</div>

---

## 🔥 Overview

This repository contains:

✔️ **n8n Workflow Library** – ready-to-import automation templates  
✔️ **AI Cookbooks for VLM Run** – notebooks and examples showing how to use the VLM Run APIs in Python and n8n

VLM Run is a developer-friendly **Visual AI platform** that enables extraction, transformation, and generation from visual data (images, documents, videos) with structured JSON outputs and visual reasoning capabilities. :contentReference[oaicite:0]{index=0}

---

## 📦 What's Inside

### 📁 Repository Structure
n8n-workflows/

├── workflows/ # n8n JSON workflows

├── ai-cookbooks/ # VLM Run Python notebooks & examples

├── assets/ # Icons, diagrams, media

├── docs/ # Extended documentation

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

