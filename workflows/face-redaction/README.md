# Face Redaction Using VLM Run Chat Completion

Automatically detect and blur human faces in images using VLM Run's visual AI for privacy protection and GDPR compliance.

## 📸 Workflow Screenshot

![Workflow Screenshot](./screenshot.png)

## 🎯 Use Case

This workflow demonstrates an end-to-end automated face redaction pipeline using VLM Run Chat Completion in n8n. Ideal for:
- Privacy protection
- Healthcare data handling
- Surveillance anonymization
- GDPR-compliant media processing

## 🔧 How It Works

1. **Input & Image Upload** – User uploads an image via Form Trigger.
2. **Upload to VLM Run** – The image is uploaded to VLM Run storage, returning a publicly accessible URL.
3. **Generate Redaction** – VLM Run Chat Completion processes the image to:
   - Detect all human faces
   - Apply blurring and redaction
   - Return a signed GCS URL for the processed image
4. **Artifact Handling** – Extracts the generated image ID using regex and fetches the artifact using session ID.
5. **Distribution** – The redacted image is:
   - Sent via Telegram
   - Uploaded to Google Drive

## 📦 Required Integrations

| Integration | Purpose |
|-------------|---------|
| **VLM Run** | Visual AI for face detection and redaction |
| **Telegram** | Send redacted images via bot |
| **Google Drive** | Store processed images |

## 🔑 VLM Run Setup

This workflow uses VLM Run for Visual AI capabilities.

1. **Get API Key**: Sign up at [app.vlm.run](https://app.vlm.run/) and create an API key
2. **Configure in n8n**: Click any VLM Run node → Create New Credential → Enter API key
3. **Operations used**:
   - `File Upload` – Upload images for processing
   - `Chat Completion` – Detect and blur faces
   - `Artifacts` – Retrieve redacted images

> 📚 [VLM Run Documentation](https://docs.vlm.run/)

## ⚙️ Setup Instructions

1. Import `workflow.json` into your n8n instance
2. Configure the following credentials:
   - VLM Run API key ([Get one here](https://app.vlm.run/))
   - Telegram Bot token and Chat ID
   - Google Drive OAuth2
3. Update the Google Drive folder ID for storage
4. Test the workflow using the Form Trigger

## 🔐 Privacy Features

- All face detection and blurring happens via VLM Run's secure API
- Pre-signed URLs ensure secure access to processed images
- No faces are stored—only redacted outputs

## 📂 Files

- `workflow.json` – The n8n workflow definition
- `README.md` – This documentation
- `screenshot.png` – Visual representation of the workflow
