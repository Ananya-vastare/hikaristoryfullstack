#  HikariStoryBoard

HikariStoryBoard is a GenAI-powered storytelling platform that transforms simple text prompts into cinematic comic-style storyboards with consistent characters, narrative flow, and AI-generated visuals.

Built for the GenAI Zürich Hackathon 2026, this project demonstrates how large language models and diffusion models can work together to create structured visual storytelling.

## Inspiration

Storytelling is one of the oldest forms of human expression, yet creating visual narratives like comics or storyboards still requires significant effort and artistic skill.

We asked:
What if anyone could turn an idea into a cinematic storyboard instantly?

HikariStoryBoard bridges the gap between imagination and visual creation using Generative AI.

## What It Does

- Converts text prompts into a 4-panel cinematic story  
- Maintains character consistency across panels  
- Generates AI-powered images for each scene  
- Adds dialogue via speech bubbles  
- Produces a complete visual storyboard  


## Architecture


<img width="165" height="150" alt="Untitled design (2)" src="https://github.com/user-attachments/assets/8650aab4-28e9-4f9f-a86e-acd42aa058f5" />


---

##  Tech Stack

Frontend:
- React + JavaScript (Vite)

Backend:
- Flask (Vercel serverless)
- Google Gemini API (story generation)
- Hugging Face SDXL (image generation)
- Pillow (image processing)

---

##  Model Selection

Story Generation:
- Gemini 2.5 Flash  
- Fast, structured output, strong narrative quality  

Image Generation:
- Stable Diffusion XL (SDXL)  
- High-quality visuals with good prompt control  

---

##  Art Style

Cinematic comic style:
- Semi-realistic  
- Dramatic lighting  
- Consistent characters  
- Graphic novel aesthetic  

Example style prompt:
cinematic comic illustration, semi-realistic, ultra detailed, dramatic lighting, consistent character design  

---

##  Challenges We Ran Into

- Maintaining character consistency  
- Getting structured JSON output from LLMs  
- Handling Vercel serverless limits  
- Fixing frontend-backend deployment issues  

---

##  Accomplishments

- Built a full LLM + Diffusion pipeline  
- Achieved consistent storytelling across panels  
- Created an AI-powered storyboard generator  

Out-of-the-box:
We built a system that understands narrative structure and visual continuity, acting like an AI storyteller and director.

---

##  What We Learned

- Prompt engineering is critical  
- Structured outputs enable multi-step AI systems  
- Deployment issues can break working systems  
- UX matters as much as AI quality  

---

##  What's Next

- Multiple art styles (anime, noir, watercolor)  
- Multi-character storytelling  
- Editable panels  
- Export as PDF/comics  
- Faster streaming responses  

---

##  Setup

Clone:
git clone <your-repo-url>  
cd hikaristoryboard  

Install:
npm install  

Run:
npm run dev  

Frontend:
http://localhost:5173  

Build:
npm run build  

---

##  Deployment

Frontend: Netlify  
Backend: Vercel  

---

##  API

https://hikaristory-backend.vercel.app/output  

---

##  Environment Variables

ACCESS_TOKEN=your_huggingface_key  
GEMINI_API_KEY=your_gemini_key  

---

## Structure

/frontend  
  /src  
    hooks/useApi.ts  
    components/  

/backend  
  /api  
    index.py  

##  Notes

- Vercel has execution time limits  
- Ensure correct API route (/output)  
- Redeploy frontend after backend changes  

## Built With
React  
TypeScript  
Flask  
Google Gemini  
Hugging Face  
Vercel  
Netlify  

---
##  Impact & SDG Alignment

HikariStoryBoard aligns with the following UN Sustainable Development Goals:

- **Quality Education** – Enhances learning through AI-generated visual storytelling  
- **Industry, Innovation and Infrastructure** – Demonstrates real-world applications of Generative AI  
- **Reduced Inequalities** – Makes creative storytelling accessible to everyone  

Additionally, it contributes to:

- **Decent Work and Economic Growth** – Supports creators with faster content generation  
- **Responsible Consumption and Production** – Encourages efficient digital-first creation workflows  
