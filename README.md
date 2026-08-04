# 🪄 Mystic Arts Tracker: Doctor Strange Shield VFX

A real-time, browser-based computer vision application that tracks hand gestures to dynamically overlay a glowing, cinematic Doctor Strange magic shield onto a live webcam feed. 

This project requires zero backend servers or installations to run. It operates entirely in the browser using JavaScript and HTML5 Canvas.

## ✨ Features

* **Real-Time Hand Tracking:** Utilizes Google's MediaPipe machine learning models to detect 21 3D landmarks on hands with high precision and low latency.
* **Gesture Recognition:** Custom math and distance calculations detect specific finger poses (e.g., closing the hand into a fist) to trigger the visual effects.
* **Dynamic Scaling & Anchoring:** The shield calculates the exact width of the user's palm in real-time to maintain perfect scale and anchors seamlessly to the wrist regardless of depth or distance from the camera.
* **Additive Blending (Glow Effect):** Uses the Canvas API `globalCompositeOperation` to strip away video backgrounds and blend pixels additively, creating a highly realistic, glowing holographic effect.
* **Glassmorphism UI:** Features a modern, responsive user interface with frosted glass panels and live status indicators that react to the AI's detection state.

## 🛠️ Tech Stack

* **Frontend:** HTML5, CSS3, Vanilla JavaScript
* **Computer Vision:** [MediaPipe Hands](https://google.github.io/mediapipe/solutions/hands.html) (via CDN)
* **Graphics:** HTML5 `<canvas>` API

## 🚀 How to Run Locally

Because web browsers restrict webcam access for local `file://` URLs for security reasons, you must run this project through a local development server.

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/dr-strange-web-magic.git](https://github.com/YOUR_USERNAME/dr-strange-web-magic.git)
   cd dr-strange-web-magic

