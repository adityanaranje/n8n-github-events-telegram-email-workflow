# 🚀 GitHub Event Automation Workflow in n8n

![n8n](https://img.shields.io/badge/n8n-Workflow-blue) ![GitHub](https://img.shields.io/badge/GitHub-Automation-green) ![LLM](https://img.shields.io/badge/LLM-Google%20Gemini-orange)

This **n8n workflow** automates the processing of **GitHub events** and sends structured notifications via **Telegram** and **Email**, leveraging **LLMs** and custom scripts for intelligent message formatting.

---

## ✨ Features

- 📌 **Listen to GitHub events:** `star`, `unstar`, `push`, `pull request`, `commit`  
- ⚡ **Data preprocessing:** Custom logic using **JavaScript** and n8n nodes  
- 🤖 **LLM-powered processing:** Uses **Google Gemini Chat Models**  
- 📝 **Output parsing:** Formats LLM responses for easy consumption  
- 📩 **Multi-channel notifications:** Send messages via  
  - **Telegram bot**  
  - **Email**  
- 🛠 **Built entirely in n8n:** No external orchestration required  

---

## 🛠 Workflow Steps

1. **GitHub Event Trigger**  
   - Automatically triggers on events like `push`, `commit`, `star`, or `pull request`.

2. **Format Response**  
   - Preprocesses the GitHub payload for LLM processing.

3. **LLM Processing**  
   - Uses **Google Gemini** models to generate formatted messages.  
   - Structured output parsing ensures notifications are clean and actionable.

4. **Edit Fields / JavaScript**  
   - Optional JS code to customize messages or perform additional processing.

5. **Send Notifications**  
   - Sends structured messages to **Telegram bot** and **Email**.  

---

## 🔧 Prerequisites

- **n8n** installed (Docker recommended)  
- **Telegram Bot API key**  
- **Gmail/SMTP credentials**  
- **Google Gemini API key**  

---

## 🚀 Installation

1. **Start n8n using Docker:**

```bash
docker run -it --rm \
  --name n8n \
  -p 5678:5678 \
  -v ~/.n8n:/home/node/.n8n \
  n8nio/n8n
```

2. **Download the workflow JSON** provided above.
    Check out the workflow and code here: [https://github.com/adityanaranje/CODEVO](https://github.com/adityanaranje/CODEVO)
    
3. **Import the workflow JSON** in n8n.
  
4. **Add credentials** for:  
   - GitHub  
   - Telegram Bot  
   - Gmail/SMTP  
   - Google Gemini LLM  

7. **Activate the workflow** and start receiving notifications.  

---

## 📈 Usage

- Once activated, this workflow listens to all configured GitHub events.  
- Notifications are sent automatically to Telegram and Email.  
- Messages are formatted and parsed for clarity and readability.

---


