# **Hale Story – Project Spec**  

## **Overview**  
Hale Story is a **local** app that generates **storyboards** with:  
- **AI images** (scene visuals)  
- **AI-generated scripts** (voiceover text)  
- **AI voice narration** (timed with visuals)  
- **Automated video assembly** (merging images & voiceover with precise timing)  

## **Core Features**  
✅ **Scene-based storytelling** (image + text per scene)  
✅ **AI-generated images & scripts**  
✅ **AI voice narration**  
✅ **Automatic timestamping** for synchronized scene transitions  
✅ **Automated merging of images & voiceover**  
✅ **Adjustable scene duration**  
✅ **Export as MP4 or storyboard (images + text)**  

## **Tech Stack**  
- **Python or Electron.js** (local app)  
- **DALL·E / Stable Diffusion** (images)  
- **GPT-4 / Claude** (scripts)  
- **TTS Options (Voiceover):**  
  - **ElevenLabs / Google TTS** *(high-quality, but requires internet & potential costs)*  
  - **NaturalReader (Desktop Version)** *(local, free option with decent quality)*  
  - **Coqui TTS** *(fully open-source & local, but requires setup)*  
  - **Piper TTS** *(lightweight & offline, great for automation)*  
- **Video Assembly (Image + Voiceover Merging):**  
  - **FFmpeg** *(automated video creation with precise timestamps)*  
  - **MoviePy** *(Python-based, easier scripting for sequencing scenes & audio)*  

## **Future Enhancements**  
- **Custom styles & user uploads**  
- **Multi-language narration**  

No backend. No authentication. Runs locally. **Fast & simple.** 🚀
