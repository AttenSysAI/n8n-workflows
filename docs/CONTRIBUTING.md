# Contributing to n8n Workflow Templates

Thank you for your interest in contributing to this repository! We welcome contributions from the community.

## 📋 Table of Contents

- [Getting Started](#getting-started)
- [Adding a New Workflow](#adding-a-new-workflow)
- [Workflow Guidelines](#workflow-guidelines)
- [Documentation Standards](#documentation-standards)
- [Submitting Your Contribution](#submitting-your-contribution)
- [Code of Conduct](#code-of-conduct)

---

## 🚀 Getting Started

1. **Fork the repository** on GitHub
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/AttenSysAI/n8n-workflows.git
   cd n8n-workflows
   ```
3. **Create a new branch** for your workflow:
   ```bash
   git checkout -b add-workflow/your-workflow-name
   ```

---

## 📁 Adding a New Workflow

### Step 1: Create the Workflow Folder

Create a new folder under `workflows/` using kebab-case naming:

```
workflows/
└── your-workflow-name/
    ├── workflow.json
    ├── README.md
    └── screenshot.png
```

**Naming conventions:**
- Use lowercase letters
- Use hyphens (`-`) to separate words
- Be descriptive but concise
- Examples: `slack-notification-bot`, `pdf-to-text-extraction`, `image-watermarking`

### Step 2: Export Your Workflow

1. Open your workflow in n8n
2. Click the **three dots menu** (⋮) in the top right
3. Select **Download**
4. Save as `workflow.json` in your workflow folder

### Step 3: Create the README

Create a `README.md` file following this template:

```markdown
# Your Workflow Name

Brief description of what this workflow does (1-2 sentences).

## 📸 Workflow Screenshot

![Workflow Screenshot](./screenshot.png)

## 🎯 Use Case

Explain the problem this workflow solves and who would benefit from it.

## 🔧 How It Works

1. **Step 1** – Description
2. **Step 2** – Description
3. **Step 3** – Description

## 📦 Required Integrations

| Integration | Purpose |
|-------------|---------|
| **Service Name** | What it's used for |

## ⚙️ Setup Instructions

1. Import `workflow.json` into your n8n instance
2. Configure the following credentials:
   - Credential 1
   - Credential 2
3. Any additional setup steps

## 📂 Files

- `workflow.json` – The n8n workflow definition
- `README.md` – This documentation
- `screenshot.png` – Visual representation of the workflow
```

### Step 4: Add a Screenshot

1. Open your workflow in n8n
2. Zoom out to show the entire workflow
3. Take a screenshot (PNG format)
4. Save as `screenshot.png` in your workflow folder

**Screenshot tips:**
- Capture the entire workflow canvas
- Use a clean background (default n8n theme)
- Ensure all nodes are visible
- Recommended width: 1200-1600px

### Step 5: Update the Main README

Add your workflow to the Workflow Index table in the root `README.md`:

```markdown
| [Your Workflow Name](./workflows/your-workflow-name/) | Brief description |
```

---

## ✅ Workflow Guidelines

### Quality Standards

- [ ] Workflow must be **tested and working**
- [ ] Remove any **sensitive data** (API keys, tokens, personal info)
- [ ] Use **descriptive node names** (not "HTTP Request", but "Fetch User Data")
- [ ] Include **Sticky Notes** in the workflow to explain complex logic
- [ ] Handle **errors gracefully** where appropriate

### Security Checklist

Before submitting, ensure you have removed:

- [ ] API keys and secrets
- [ ] Personal email addresses
- [ ] Webhook URLs with tokens
- [ ] Database connection strings
- [ ] OAuth tokens and credentials
- [ ] Any personally identifiable information (PII)

### Best Practices

1. **Use environment variables** for configurable values
2. **Add error handling** nodes for critical operations
3. **Include sample data** in Sticky Notes if helpful
4. **Group related nodes** logically
5. **Use consistent naming** for nodes and variables

---

## 📝 Documentation Standards

### README Requirements

Every workflow README must include:

| Section | Required | Description |
|---------|:--------:|-------------|
| Title & Description | ✅ | Clear name and one-line summary |
| Screenshot | ✅ | Visual preview of the workflow |
| Use Case | ✅ | Who needs this and why |
| How It Works | ✅ | Step-by-step explanation |
| Required Integrations | ✅ | Table of services needed |
| Setup Instructions | ✅ | How to configure and run |
| Files | ✅ | List of files in the folder |

### Optional Sections

- **Output Schema** – For workflows that return structured data
- **Customization** – Tips for modifying the workflow
- **Troubleshooting** – Common issues and solutions
- **Related Workflows** – Links to similar workflows

### Writing Style

- Use clear, concise language
- Write in second person ("you", "your")
- Use bullet points and tables for readability
- Include code blocks for commands and JSON
- Add emoji sparingly for visual hierarchy

---

## 🔄 Submitting Your Contribution

### Before Submitting

1. **Test your workflow** thoroughly
2. **Review the security checklist** above
3. **Ensure documentation is complete**
4. **Check that screenshot is clear and readable**

### Creating a Pull Request

1. **Commit your changes:**
   ```bash
   git add .
   git commit -m "Add workflow: your-workflow-name"
   ```

2. **Push to your fork:**
   ```bash
   git push origin add-workflow/your-workflow-name
   ```

3. **Open a Pull Request** on GitHub with:
   - Clear title: `Add workflow: Your Workflow Name`
   - Description of what the workflow does
   - Any special setup requirements
   - Screenshots if helpful

### PR Review Process

1. A maintainer will review your PR
2. They may request changes or clarifications
3. Once approved, your workflow will be merged
4. Your contribution will be credited

---

## 🤝 Code of Conduct

### Our Standards

- Be respectful and inclusive
- Provide constructive feedback
- Focus on the work, not the person
- Help others learn and grow

### Unacceptable Behavior

- Harassment or discrimination
- Trolling or insulting comments
- Publishing others' private information
- Other unprofessional conduct

---

## 💬 Getting Help

If you have questions or need help:

- **Discord:** [Join our community](https://discord.gg/v3rTUufp)
- **Twitter:** [@AttenSysAI](https://x.com/AttenSysAI)
- **GitHub Issues:** Open an issue for bugs or feature requests

---

## 🙏 Thank You!

Your contributions help make this repository better for everyone. We appreciate your time and effort!
