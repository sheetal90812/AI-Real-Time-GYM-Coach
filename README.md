# 🏋️ AI Real-Time GYM Coach
**Real-time AI fitness coaching using Computer Vision, Pose Estimation, WebRTC, and Generative AI.**
AI Real-Time GYM Coach is an intelligent fitness assistant that analyzes workout movements through a live camera, detects body poses, counts repetitions and sets, monitors exercise-specific metrics, and provides AI-generated coaching feedback with voice assistance.
The application combines **MediaPipe Pose Landmarker, WebRTC, Streamlit, Groq AI, Text-to-Speech, and SQLite** into a complete real-time fitness application.

## 🌐 Live Demo
🚀 **Live Application:**
https://ai-real-time-gym-coach-production.up.railway.app/

📦 **GitHub Repository:**
https://github.com/sheetal90812/AI-Real-Time-GYM-Coach

# 📌 Project Overview
Traditional workout applications often depend on manual repetition tracking or pre-recorded instructions.
The **AI Real-Time GYM Coach** provides a more interactive approach by using computer vision to analyze a user's movement through a webcam.
The system:
1. Captures live video from the user's camera.
2. Establishes a real-time WebRTC connection.
3. Detects human body landmarks using MediaPipe Pose Landmarker.
4. Analyzes exercise-specific joint movements.
5. Counts repetitions automatically.
6. Tracks sets and workout progress.
7. Generates contextual AI coaching feedback.
8. Provides voice-based coaching.
9. Stores workout history for the user.

# ✨ Key Features
## 🎥 Real-Time Pose Detection
* Live webcam-based exercise tracking
* Real-time human pose landmark detection
* MediaPipe Pose Landmarker integration
* Continuous movement analysis

## 🔢 Automatic Rep & Set Tracking
* Automatic repetition counting
* Current set tracking
* Total repetition tracking
* Completed set tracking
* Workout completion detection

## 🏋️ Supported Exercises
The current application supports:
* 🏋️ Squats
* 💪 Push-ups
* 🏋️ Biceps Curls (Dumbbell)
* 🏋️ Shoulder Press
* 🦵 Lunges

---

# 📊 Exercise-Specific Metrics
Different exercises use different movement metrics to analyze movement and form.

### Squats
* Knee Angle
* Back Angle
* Depth Status

### Push-ups
* Elbow Angle
* Body Alignment
* Hip Position

### Biceps Curls
* Elbow Angle
* Shoulder Stability
* Swing Detection

### Shoulder Press
* Elbow Angle
* Arm Extension
* Back Arch

### Lunges
* Front Knee Angle
* Torso Angle
* Balance Status

---

# 🤖 AI Coaching
The application integrates **Groq-powered Generative AI** to provide contextual coaching feedback during workouts.
The coaching system can respond to workout events such as:
* Workout started
* Exercise progress
* Set progress
* Workout completion
Example:
> 🤖 **Coach:** Nice work! Keep that intensity up through the next rep!
The goal is to make the application behave more like an **interactive virtual fitness assistant** rather than a simple repetition counter.

# 🔊 Voice Coaching
The project includes a voice pipeline combining:
* AI-generated coaching
* Text-to-Speech
* Automatic audio playback
This allows users to receive coaching feedback while exercising instead of constantly looking at the screen.

# 👤 User Login
The application includes a login system that associates workout activity with the logged-in user.
This allows workout history to be displayed for individual users.

# 💾 Workout History
Workout information is stored using **SQLite**, allowing the application to maintain workout-related data and display previous workout activity.

# 🏗️ System Architecture

                         USER
                           │
                           ▼
                  ┌─────────────────┐
                  │ Browser Camera  │
                  └────────┬────────┘
                           │
                           ▼
                  ┌─────────────────┐
                  │     WebRTC      │
                  │ Live Video Feed │
                  └────────┬────────┘
                           │
                           ▼
                  ┌─────────────────┐
                  │  MediaPipe Pose │
                  │    Landmarker   │
                  └────────┬────────┘
                           │
                           ▼
                  ┌─────────────────┐
                  │ Movement / Pose │
                  │    Analysis     │
                  └────────┬────────┘
                           │
                 ┌─────────┴─────────┐
                 │                   │
                 ▼                   ▼
        ┌─────────────────┐   ┌─────────────────┐
        │ Rep / Set       │   │ Exercise        │
        │ Tracking        │   │ Metrics         │
        └────────┬────────┘   └────────┬────────┘
                 │                     │
                 └──────────┬──────────┘
                            │
                            ▼
                   ┌─────────────────┐
                   │ Workout Events  │
                   └────────┬────────┘
                            │
                            ▼
                   ┌─────────────────┐
                   │   AI Coaching   │
                   │    Groq LLM     │
                   └────────┬────────┘
                            │
                            ▼
                   ┌─────────────────┐
                   │ Text-to-Speech  │
                   └────────┬────────┘
                            │
                            ▼
                   ┌─────────────────┐
                   │ Voice Feedback  │
                   └─────────────────┘

                            │
                            ▼
                   ┌─────────────────┐
                   │ Workout History │
                   │     SQLite      │
                   └─────────────────┘

# 🛠️ Tech Stack

<img width="682" height="658" alt="image" src="https://github.com/user-attachments/assets/9074e760-f6c7-4a97-a235-24187554ae64" />

# 🎯 Project Goal
The goal of this project was to explore how **computer vision, real-time video processing, and generative AI** can be combined to create an interactive fitness assistant.
Instead of simply displaying workout instructions, the system processes the user's movement, tracks workout progress, and provides personalized coaching feedback during the session.

## 👨‍💻 Author
**Sheetal**

Computer Science Engineering Student
Interested in **AI Engineering, Generative AI, Computer Vision, LLMs, and Agentic AI**.
