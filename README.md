# 🎬 HikariStoryBoard

HikariStoryBoard is a GenAI-powered storytelling platform that transforms simple text prompts into cinematic comic-style storyboards with consistent characters, narrative flow, and AI-generated visuals.

Built for the **GenAI Zürich Hackathon 2026**, this project demonstrates how large language models and diffusion models can work together to create structured visual storytelling.

---

## 🚀 Tech Stack

### Frontend
- React + TypeScript (Vite)
- Custom hooks for API handling
- Responsive UI for storyboard visualization

### Backend
- Flask (deployed on Vercel serverless)
- Google Gemini (story generation)
- Hugging Face (image generation - Stable Diffusion XL)

---

## 🧠 Core Features

- ✍️ Prompt → Story (LLM-based narrative generation)
- 🎭 Character Consistency across panels
- 🎨 AI-generated cinematic comic visuals
- 💬 Speech bubble rendering on images
- ⚡ Real-time API interaction with loading + error handling

---

## ⚙️ Development Setup

### 1. Clone the repo

### 2. Install dependencies
   ````
npm install

### 3. Run locally
````
npm run dev

Frontend runs on:
`````
http://localhost:5173

### 4. Build for production
 ````
npm run build

### Deployment
Frontend
Hosted on Netlify

Backend
Hosted on Vercel (serverless Flask API)

Add:
ACCESS_TOKEN=your_huggingface_key
GEMINI_API_KEY=your_gemini_key
🧩 Project Structure
/frontend
  /src
    hooks/useApi.ts
    components/
    pages/

backend (vercel)
/api
  index.py
Notes

Vercel serverless functions have execution limits (important for image generation)

Ensure correct API routes (/output or /api/output)

Always redeploy frontend after API changes

### Future Improvements

Streaming responses for faster UX

Multi-character storytelling

Style selection (anime, noir, watercolor)

Story editing + panel regeneration

Export as PDF / comic strip

### Built With
React
TypeScript
Flask

Google Gemini API

Hugging Face Inference API

Vercel

Netlify

Team

Built during GenAI Zürich Hackathon 2026

---




```bash
git clone <your-repo-url>
cd hikaristoryboard
