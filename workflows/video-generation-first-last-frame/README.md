# Video Generation from First Frame and Last Frame using VLM Run

Generate smooth transition videos between two input frames using VLM Run's visual AI. Perfect for creative video effects and morphing animations.

## 📸 Workflow Screenshot

![Workflow Screenshot](./screenshot.png)

## 🎯 Use Case

This workflow generates smooth transition videos between two frames:
- Downloads start and end frames from URLs
- Uploads to VLM Run for processing
- Creates video with natural progression
- Returns downloadable video file

## 🔧 How It Works

1. **Input Frames** – Downloads the first (start) and last (end) frames from predefined URLs as JPEG files.
2. **Upload to VLM Run** – Uploads both frame files to VLM Run service, returning `public_url` for each frame that can be referenced in API calls.
3. **URL Extraction** – Extracts public URLs from upload responses:
   - `startFrameUrl` – URL for start frame
   - `endFrameUrl` – URL for end frame
   - Adds `frameType` field for identification
4. **Merge Frame URLs** – Combines start and end frame URLs into a single object ready for video generation.
5. **Video Generation** – VLM Run Chat Completion receives both frame URLs and creates:
   - Smooth transition video
   - Maintains exact first/last frames
   - Natural intermediate frame progression
6. **Artifact Handling** – Retrieves the generated video using session ID and object ID from the model's structured JSON response.

## 📦 Required Integrations

| Integration | Purpose |
|-------------|---------|
| **VLM Run** | Visual AI for video generation |

## 🔑 VLM Run Setup

This workflow uses VLM Run for Visual AI capabilities.

1. **Get API Key**: Sign up at [app.vlm.run](https://app.vlm.run/) and create an API key
2. **Configure in n8n**: Click any VLM Run node → Create New Credential → Enter API key
3. **Operations used**:
   - `File Upload` – Upload start and end frames
   - `Chat Completion` – Generate transition video
   - `Artifacts` – Retrieve generated video

> 📚 [VLM Run Documentation](https://docs.vlm.run/)

## ⚙️ Setup Instructions

1. Import `workflow.json` into your n8n instance
2. Configure VLM Run API credentials ([Get one here](https://app.vlm.run/))
3. Update the start and end frame URLs in the HTTP Request nodes
4. Test the workflow using the Manual Trigger

## 📋 Output Schema

The workflow returns structured output with:

```json
{
  "url": "url_xxxxx",
  "message": "..."
}
```

## 🎬 Video Features

- Smooth interpolation between frames
- Exact preservation of first and last frames
- Natural, continuous progression
- Downloadable video file output

## 📂 Files

- `workflow.json` – The n8n workflow definition
- `README.md` – This documentation
- `screenshot.png` – Visual representation of the workflow
