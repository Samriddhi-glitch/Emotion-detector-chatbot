
# 🧠 Emotion Detector Chatbot

A lightweight emotion detection tool powered by a local LLM (e.g., Mistral via Ollama). Given any input text, it returns the **primary emotion** from a defined set — quickly, privately, and with high accuracy.

---

## 🚀 Features

- 🔍 Detects the **dominant emotion** from user input
- 🛡️ Runs locally using your own LLM (no internet required)
- ⚡ Fast and privacy-friendly — no external API calls
- 🔄 Easily customizable emotion list and model

---

## 🧠 Supported Emotions

```text
joy, excitement, love, contentment, pride, relief,
sadness, anger, fear, disgust, guilt, shame,
surprise, awe, curiosity, calm, neutral, confusion
````

---

## 🔧 Requirements

* Python 3.x
* [`requests`](https://pypi.org/project/requests/)
* A local language model serving API (like [Ollama](https://ollama.com/)) running a model such as `mistral`

---

## 📦 Installation

```bash
pip install requests
```

Start your local model (example using Ollama):

```bash
ollama run mistral
```

---

## 📄 Usage

```python
from emotion_detector import detect_full_emotion

text = "I just got accepted into my dream university!"
emotion = detect_full_emotion(text)
print(emotion)  # 🧠 Detected Emotion: joy
```

---

## 🔍 Function Overview

```python
def detect_full_emotion(text, model_name="mistral"):
    ...
```

* `text`: Input string to analyze
* `model_name`: (Optional) Local model to use (default: `mistral`)

---

## 🧪 Example Output

```text
Input: "I feel like everything is falling apart."
Output: 🧠 Detected Emotion: sadness
```

---

## 📁 File Structure

```
emotion_detector/
├── emotion_detector.py
└── README.md
```

---

## 🤝 License

MIT License — feel free to use, modify, and share.

---

## ✨ Credits

Built with ❤️ using [Ollama](https://ollama.com/) and local LLMs.

```

---

Let me know if you'd like:
- A `requirements.txt`
- Streamlit or Flask frontend
- GitHub badges (Python version, license, etc.)
```
