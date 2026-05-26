# 🎬 Automate Video Creation with Veo3 & Auto-Post to Social Media

> A fully automated n8n workflow that turns a single daily prompt into a cinematic AI-generated video and publishes it across **9 social platforms** — all without lifting a finger.

<img width="566" height="617" alt="image" src="https://github.com/user-attachments/assets/4acb1574-a632-44b6-a459-15582816752a" />

---

## 📌 Who Is This For?

This template is built for:

- 🎥 **Content creators** scaling short-form video output
- 📱 **Social media managers** running multi-platform campaigns
- ▶️ **YouTubers & Shorts creators** wanting daily, consistent uploads
- 📊 **Digital marketers** automating brand presence
- 🚀 **Anyone** who wants to scale content creation **without touching video editing tools**

If you've ever felt overwhelmed by the daily grind of ideation → scripting → editing → posting, this workflow is for you.

---

## ❓ What Problem Does This Solve?

Producing consistent video content traditionally requires:

- 💡 Generating fresh ideas
- ✍️ Writing scripts and prompts
- 🎞️ Rendering videos
- 📤 Manually posting to each platform

This workflow automates **every single step**. One prompt becomes a professional AI-generated video, distributed automatically — saving hours of work and dramatically expanding your reach.

---

## ⚙️ What This Workflow Does

| Step | Action |
|------|--------|
| 1️⃣ | Triggers daily to generate a new idea with **OpenAI** (or your custom prompt) |
| 2️⃣ | Creates a video prompt formatted specifically for **Google Veo3** |
| 3️⃣ | Generates a cinematic video using the **Veo3 API** |
| 4️⃣ | Logs the video data into a **Google Sheet** |
| 5️⃣ | Retrieves the final video URL once Veo3 finishes rendering |
| 6️⃣ | Uploads the video to **Blotato** for publishing |
| 7️⃣ | Auto-posts to **Instagram, TikTok, YouTube, Facebook, LinkedIn, Threads, X (Twitter), Pinterest, and Bluesky** |

---

## 🛠️ Setup Instructions

Follow these steps to get the workflow running:

### 1. OpenAI API Key
Add your OpenAI API key to the **GPT-4.1 nodes** to enable idea and prompt generation.

### 2. Veo3 API Credentials
Connect your **Veo3 API credentials** in the video generation node.

### 3. Google Sheets
Link your Google Sheets account and prepare a sheet with the following columns:

| Column | Purpose |
|--------|---------|
| `Prompt` | The generated video idea/prompt |
| `Video URL` | The rendered Veo3 video link |
| `Status` | Current step in the pipeline |

### 4. Blotato Integration
- Connect your **Blotato API key**
- Set your **platform IDs** in the `Assign Social Media IDs` node

### 5. Schedule Trigger
Adjust the **Schedule Trigger** node to match your desired posting frequency (e.g., daily at 9 AM).

---

## 🎨 How to Customize

This workflow is designed to be flexible. Here are some ways to tailor it:

- **🎯 Niche targeting** — Edit the AI prompt to align with your topic (fitness, finance, education, real estate, etc.)
- **🖼️ Branding** — Add your own overlays, watermarks, or intros using **JSON2Video** or similar tools
- **🌐 Platform control** — Enable or disable specific HTTP Request nodes to choose which platforms receive content
- **👀 Preview before posting** — Add a **Telegram** node to review and approve videos before they go live
- **📈 Performance tracking** — Add metrics columns (views, likes, shares) in Google Sheets to monitor results

---

## 🔌 Supported Platforms

This workflow publishes to:

- 📸 Instagram
- ▶️ YouTube
- 👍 Facebook
- 💼 LinkedIn
- 🧵 Threads
- 🐦 X (Twitter)
- 📌 Pinterest
- ☁️ Bluesky

---

## 📋 Requirements

- An active **n8n** instance (cloud or self-hosted)
- **OpenAI API** account
- **Veo3 API** access (Google)
- **Blotato** account with connected social profiles
- **Google account** for Sheets integration

---

## 💡 Tips for Best Results

- Start with a **niche-specific prompt** for consistency in your content style
- Use Google Sheets to **track which prompts perform best** and refine your strategy
- Run the workflow on a **fixed schedule** to maintain algorithmic consistency
- Always **review the first few outputs** before letting it run fully autonomously
