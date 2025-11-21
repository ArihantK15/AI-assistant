# AI Voice Assistant (Gemini Integration)

A smart voice assistant written in Python that integrates **Google's Gemini API** for conversational intelligence. This assistant can perform web automation tasks, tell jokes, and answer general queries using Generative AI.

## 🚀 Features

* **Generative AI Conversations:** Uses Google's `gemini-2.5-flash-lite` model to answer complex questions and chat.
* **YouTube Integration:** verbal command "YouTube [video name]" automatically searches and plays videos.
* **Wikipedia Search:** verbal command "Wikipedia [topic]" reads a summary of the topic.
* **Entertainment:** Can tell jokes using the `pyjokes` library.
* **Natural Text-to-Speech:** Uses `gTTS` (Google Text-to-Speech) for high-quality voice output.
* **Personalized Greeting:** Greets the user based on the time of day.

## 🛠️ Tech Stack

* **Python 3.x**
* **Google Generative AI SDK** (Gemini)
* **SpeechRecognition** (Google Speech API)
* **gTTS** (Google Text-to-Speech)
* **PyWhatKit** (YouTube automation)
* **Wikipedia API**

## 📋 Prerequisites

### System Requirements
**Note:** This script currently uses `afplay`, which is a command-line audio player native to **macOS**.
* If you are on **Windows** or **Linux**, you will need to modify the `speak()` function to use `playsound` or `os.system("start ...")`.

### API Key
You will need a valid API Key from Google AI Studio.
1.  Go to [Google AI Studio] (https://aistudio.google.com/).
2.  Create an API key.

## 📦 Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/yourusername/your-repo-name.git](https://github.com/yourusername/your-repo-name.git)
    cd your-repo-name
    ```

2.  **Install the required dependencies:**
    ```bash
    pip install speechrecognition pyttsx3 wikipedia pyjokes google-generativeai gTTS pywhatkit pyaudio
    ```
    *(Note: `pyaudio` is required for microphone input. On some systems, you may need to install `portaudio` via Homebrew or apt-get first).*

3.  **Configure your API Key:**
    Open the Python script and replace the placeholder with your actual key:
    ```python
    api_key = "YOUR_GOOGLE_GEN_AI_KEY_HERE"
    ```

## 💻 Usage

Run the main script:

```bash
python main.py
