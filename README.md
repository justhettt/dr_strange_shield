

---

```markdown
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

```

2. **Start a local server:**
If you have Python installed (macOS/Linux usually do by default), run:
```bash
python3 -m http.server 8000

```


*Alternatively, you can use the Live Server extension in VS Code.*
3. **Open the app:**
Navigate to `http://localhost:8000` in your web browser (Chrome or Safari recommended). Grant camera permissions when prompted.

## 🌐 Live Deployment (GitHub Pages)

This project is purely frontend, making it incredibly easy to host for free via GitHub Pages.

1. Fork or upload this repository to your GitHub account.
2. Navigate to your repository **Settings**.
3. On the left sidebar, click **Pages**.
4. Under "Build and deployment", select **Deploy from a branch**.
5. Choose the `main` branch and click **Save**.
6. Within a few minutes, your magical web app will be live at `https://yourusername.github.io/dr-strange-web-magic`!

## 📁 File Structure

* `index.html`: Contains the core application structure, the Glassmorphism CSS UI, and the JavaScript logic for MediaPipe and Canvas rendering.
* `shield.mp4`: The VFX video asset used for the magic shield effect (Must have a black background for additive blending).

## 🧙‍♂️ How to Use the App

1. Stand in a well-lit room so the camera can clearly see your hands.
2. Hold your hand up to the camera with your fingers open. The UI will indicate it is tracking you.
3. **Close your hand into a tight fist** to cast the spell and summon the shield!

```

```
