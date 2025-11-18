
# Word Builder (OpenCV + MediaPipe)

Turn hand gestures into speculative worlds.
Word Builder is an interactive prototype inspired by the idea of “an infinite word builder with gestures.”

Point at on-screen dials, pinch to tweak three sliders — Biology, Technology, Culture — then hold an open palm for ~1 second to generate a brand-new world title and description.

Runs locally using OpenCV + MediaPipe, and can optionally call an LLM (Gemini or OpenAI) if you provide an API key.

## ✨ Features

🖐 Real-time hand tracking with MediaPipe Hands

🎛 Three neon-style HUD dials:

* Biology

* Technology

* Culture

🎯 Gesture controls:

* Pinch to grab and adjust dials

* Open palm to trigger world generation

🤖 LLM-backed world generator:

* Supports Gemini 1.5 Flash or OpenAI

* Falls back to a deterministic local generator if no API key is set

🧠 Runs entirely on your machine using your webcam

# 🚀 Setup (Windows PowerShell)

From the project root:
``` # 1) Create and activate a virtual environment (recommended)
python -m venv .venv
.\.venv\Scripts\Activate.ps1

# 2) Install dependencies
pip install -r requirements.txt

# 3) (Optional) Set an API key for LLM text

# For Gemini:
$env:GEMINI_API_KEY = "<your_key>"

# Or for OpenAI:
$env:OPENAI_API_KEY = "<your_key>"
```

# ▶️ Run the App
```
python -m app.main --camera 0 --width 1280 --height 720
```
