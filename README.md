<img width="3188" height="1202" alt="frame (3)" src="https://github.com/user-attachments/assets/517ad8e9-ad22-457d-9538-a9e62d137cd7" />


# Mooku_lipi (the nose script) 🎯


## Basic Details
### Team Name: TechLet


### Team Members
- Team Lead: Shaheem
- Member 2: Sajin


### Project Description
Mooku_Lipi is an interactive, real-time Malayalam handwriting learning and evaluation tool that lets users draw Malayalam letters using nose tracking via webcam. By leveraging MediaPipe’s face mesh technology, the app tracks the user’s nose movements to allow drawing on the screen without touching any device.

The project uses advanced image processing and AI-powered analysis (via Gemini API) to compare the user’s drawing with reference letters, providing instant feedback on accuracy, along with funny and encouraging Malayalam comments. This engaging approach helps users, especially children, improve their Malayalam handwriting skills in a fun, gamified way with particle effects and friendly UI prompts.

Ideal for language learners, educators, and enthusiasts, Mooku_Lipi blends computer vision, AI, and cultural language preservation into a novel educational experience.

### The Problem (that doesn't exist)
Who knew learning Malayalam handwriting could be so boring? Holding a pen and paper is so last century, and no one wants to squint over textbooks or practice sheets—especially kids! Plus, nobody has time to get a handwriting coach who can laugh at your mistakes with you.

### The Solution (that nobody asked for)
Introducing Mooku_Lipi — the world’s first Malayalam handwriting app you control with your nose! That’s right, just wave your nose in front of your webcam, and start drawing letters in the air. Our AI-powered magic compares your nose-art with perfect letters, gives you hilarious Malayalam comments to keep you smiling, and sprinkles cool particle explosions for every stroke. Learning Malayalam writing just got a whole lot sillier... and way more fun!

## Technical Details

### Technologies/Components Used

#### For Software:
- **Languages used:** Python
- **Frameworks used:** None (uses OpenCV, Pygame, MediaPipe libraries)
- **Libraries used:**  
  - OpenCV  
  - MediaPipe  
  - Pygame  
  - Pillow (PIL)  
  - Requests  
  - Scikit-image (for SSIM)  
- **Tools used:**  
  - Python interpreter  
  - Git for version control  
  - Gemini API for handwriting analysis






## Project Documentation

### For Software

**1. Overview**  
**Mooku_Lipi** is a computer vision–based Malayalam handwriting learning tool that uses nose tracking to draw letters in the air. The system captures webcam input, tracks the user's nose tip, renders drawing strokes, and compares them against reference Malayalam letters using AI-powered evaluation and offline similarity metrics.

---

**2. Architecture**

**Core Components:**  
1. **Webcam Input** – Captures real-time video feed using OpenCV.  
2. **Face Mesh Tracking** – Uses MediaPipe to identify and track the nose tip position.  
3. **Drawing Engine** – Renders virtual strokes with particle effects using Pygame.  
4. **Letter Display Module** – Displays randomly selected Malayalam letters to be drawn.  
5. **Evaluation Module** –  
   - **Primary:** Google Gemini API for AI accuracy scoring  
   - **Fallback:** SSIM-based image similarity for offline evaluation  
6. **Audio Feedback System** – Uses gTTS to speak instructions and results in Malayalam.  
7. **Font Rendering** – Loads Malayalam Unicode fonts with PIL for cross-platform display.

---

**3. Workflow**

1. **Startup:**  
   - Initialize webcam, load fonts, prepare letter set, and display instructions.

2. **Gameplay Loop:**  
   - Show a random Malayalam letter.  
   - Track nose position and draw strokes on the canvas.  
   - Apply particle effects for visual feedback.

3. **Evaluation:**  
   - When the user indicates completion, the drawn image is compared with the reference.  
   - If Gemini API is available, send the images for AI scoring.  
   - If Gemini fails or no internet, fall back to SSIM similarity calculation.

4. **Feedback:**  
   - Display the score visually.  
   - Speak the feedback in Malayalam via gTTS.

5. **Repeat:**  
   - Move to the next letter until the session ends.

---

**4. File Structure**
Mooku_Lipi/
│
├── mooku_lipi.py # Main application code\n
├── fonts/ # Malayalam font files
├── assets/ # Images or additional resources
├── requirements.txt # Dependencies
├── README.md # Project description and usage

**5. Dependencies**

- Python 3.7+  
- OpenCV  
- MediaPipe  
- Pillow (PIL)  
- NumPy  
- scikit-image  
- gTTS  
- Requests  
- Pygame  

---

## 6. Setup Instructions

```bash
git clone https://github.com/<yourusername>/Mooku_Lipi.git
cd Mooku_Lipi
pip install -r requirements.txt
python mooku_lipi.py
```








---
Made with ❤️ at TinkerHub Useless Projects 

![Static Badge](https://img.shields.io/badge/TinkerHub-24?color=%23000000&link=https%3A%2F%2Fwww.tinkerhub.org%2F)
![Static Badge](https://img.shields.io/badge/UselessProjects--25-25?link=https%3A%2F%2Fwww.tinkerhub.org%2Fevents%2FQ2Q1TQKX6Q%2FUseless%2520Projects)



