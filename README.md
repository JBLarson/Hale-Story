# **Hale Story – Project Spec**  

## **Overview**  
Hale Story is a **local** app that generates **storyboards** with:  
- **AI-generated stories** (based on classic fables and childhood tales)  
- **AI-generated images** (characters and scenes based on the story)  
- **AI-generated voice narration** (scripted and timed for natural flow)  
- **Automated timing suggestions** (determining how long each image is displayed)  
- **Manual video assembly** (combining images, narration, and captions into a final video)  

## **Workflow**  
### **Step 1: Story Generation**  
1. Provide an **LLM (GPT-4/Claude)** with a structured **story template** (inspired by a classic fable like *The Tortoise and the Hare*).  
2. The LLM generates a **full story** with clear scenes.  

### **Step 2: Character & Scene Definition**  
1. The LLM analyzes the story and creates a **character characteristics chart** for use with **Stable Diffusion** (e.g., descriptions, styles, key traits).  
2. The LLM also defines **scene descriptions** for generating AI images.  

### **Step 3: Image Generation**  
1. Use **Stable Diffusion** to generate **images** for each scene based on the character and scene descriptions.  

### **Step 4: Voiceover Script & Timing**  
1. The LLM generates a **TTS-friendly script** for narration.  
2. The script is optimized for **150 words per minute (wpm)** speech pace.  
3. The LLM provides **suggested display durations** for each scene.  

### **Step 5: Manual Video Assembly**  
1. Manually combine the **generated images** and **text-to-speech (TTS) narration** into a video.  
2. Add **captions** for accessibility.  

### **Step 6: Export & Review**  
1. Export the final video as **MP4** or a **storyboard format** (images + text).  
2. Review and refine as needed.  

## **Core Features**  
✅ **Story generation from a classic fable template**  
✅ **AI-generated images (characters & scenes)**  
✅ **AI voice narration (scripted & timed)**  
✅ **TTS pacing at 150 wpm for smooth narration**  
✅ **LLM-suggested scene display durations**  
✅ **Manual merging of images, voiceover, and captions**  
✅ **Export as MP4 or storyboard (images + text)**  

## **Tech Stack**  
- **Python or Electron.js** (local app)  
- **Stable Diffusion** (AI-generated images)  
- **GPT-4 / Claude** (story & script generation)  
- **TTS Options (Voiceover):**  
  - **ElevenLabs / Google TTS** *(high-quality, requires internet & potential costs)*  
  - **NaturalReader (Desktop Version)** *(local, free option with decent quality)*  
  - **Coqui TTS** *(open-source & local, requires setup)*  
  - **Piper TTS** *(lightweight & offline, good for automation)*  
- **Video Assembly (Image + Voiceover Merging):**  
  - **FFmpeg** *(precise timestamp-based automation)*  
  - **MoviePy** *(Python-based, easier scripting for sequencing scenes & audio)*  

## **Future Enhancements**  
- **Custom styles & user uploads**  
- **Multi-language narration**  

No backend. No authentication. Runs locally. **Fast & simple.** 🚀  
