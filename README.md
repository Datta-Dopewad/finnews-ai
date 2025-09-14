# 📈 FinNews AI – Daily Financial News Summarizer

Receive curated **Financial Times (FT.com) market news** directly into your **Microsoft Outlook inbox every morning**.  
This project uses **n8n workflow automation + OpenAI API** to fetch, summarize, and deliver investor-ready financial updates.

---

## 🚀 Features
- ⏰ Automatic daily trigger at 7:00 AM
- 🌐 Fetches latest headlines & sections from [FT.com](https://www.ft.com/)
- 🧠 Summarizes news into **clear, concise investor insights** using OpenAI API
- 📧 Sends structured **HTML email** via Microsoft Outlook
- 📊 Ready for investors, students, and professionals who want quick financial updates

---

## 🏗️ Architecture

**Workflow Steps:**
1. **Schedule Trigger** – runs every day at 7:00 AM
2. **HTTP Request** – fetches FT.com financial news HTML
3. **HTML Extractor** – extracts sections (Headlines, Editor’s Picks, Market Spotlight)
4. **Aggregator Node** – combines extracted data
5. **AI Summarizer** – uses OpenAI API to create investor-friendly summary
6. **Outlook Node** – sends HTML email with structured news

📌 See `docs/architecture-diagram.png` for the workflow visualization.

---

## 📥 Installation & Setup

### 1. Clone the repo
```bash
git clone https://github.com/Datta-Dopewad/finnews-ai
