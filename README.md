<div align="center"> <p align="center" style="width: 100%;"> <img src="https://raw.githubusercontent.com/vlm-run/.github/refs/heads/main/profile/assets/vlm-black.svg" alt="VLM Run Logo" width="80" style="margin-bottom: -5px; vertical-align: middle; padding-right: 5px;"><br> </p> <h2>VLM Run AI Cookbooks</h2> <p align="center"> <a href="https://vlm.run"><b>Website</b></a> | <a href="https://app.vlm.run/"><b>Platform</b></a> | <a href="https://github.com/vlm-run/vlmrun-hub"><b>Hub</b></a> | <a href="https://docs.vlm.run/"><b>Docs</b></a> | <a href="https://vlm.run/blog"><b>Blog</b></a> | <a href="https://discord.gg/AMApC2UzVY"><b>Discord</b></a> </p> <p align="center"> <a href="https://discord.gg/AMApC2UzVY"><img alt="Discord" src="https://img.shields.io/badge/discord-chat-purple?color=%235765F2&label=discord&logo=discord"></a> <a href="https://twitter.com/vlmrun"><img alt="Twitter Follow" src="https://img.shields.io/twitter/follow/vlmrun.svg?style=social&logo=twitter"></a> </p> </div>

🔥 What’s Inside
✅ n8n Workflow Library

Google Drive → AI pipelines

Image redaction & annotation

Audio/video-to-text pipelines

Text + image hybrid data workflows

Automated meeting summarization

Document OCR + vector extraction

Custom webhook-trigger automations

🤖 AI Workflows with VLM Run

Image-to-image style transfer

Photo → painting conversions

Artistic variations

Batch image transformation

Professional headshot generation (19 camera angles)

Vision-language hybrid answering

Image-based reasoning & data extraction

📚 Learn the Docs — VLM Run Platform

This repo includes cookbooks demonstrating how to use VLM Run’s image-to-image agent in Python.

🧩 Prerequisites

Python 3.10+

API Key: VLMRUN_API_KEY
(Get one from https://app.vlm.run
 )

Install packages:

pip install vlmrun[openai] cachetools pillow requests numpy

▶ Running the Notebooks
In Google Colab

Click the Colab badge next to each notebook.

Locally (Jupyter)

Ensure Python 3.10+

Set VLMRUN_API_KEY

Open .ipynb → run cells top-to-bottom

📒 Cookbooks
Name	Type	Colab
Image-to-Image Style Transfer
	<kbd>image-to-image</kbd>	

Professional Headshot Generation (19 Angles)
	<kbd>image-gen</kbd>	

Reminder: Replace <YOUR_ORG>/<YOUR_REPO> after pushing the repo.

📂 Repository Structure
n8n-workflows/
 ├── workflows/              # n8n JSON workflows
 ├── ai-cookbooks/           # VLM Run image notebooks
 ├── assets/                 # Icons, diagrams, media
 ├── docs/                   # Documentation extensions
 └── README.md

⚙️ Setup
1️⃣ Install n8n

https://docs.n8n.io/installation

2️⃣ Import Workflows

n8n → Import → upload JSON from /workflows

3️⃣ Configure API Keys

Depending on workflow:

VLM Run

Google Drive

OpenAI-style agents

Notion / Sheets / Slack

Webhooks

🆘 Support & Resources
📖 Docs

https://docs.vlm.run/

💬 Discord

https://discord.gg/AMApC2UzVY

🐦 Twitter

https://twitter.com/vlmrun

⭐ Contributing

Pull requests welcome!
You can add:

New n8n workflows

Image/AI pipelines

Integration templates

Cookbook notebooks

If you want, I can also provide:

✅ Badge pack (stars, license, build, AI-powered)
✅ Workflow diagrams (Mermaid / PNG)
✅ A "Quickstart" GIF animation for the repo
✅ A logo header matching VLM styling
