🎙️ Mini Voice Assistant (Python)
This is a simple Python-based voice assistant that can open commonly used applications or search the web using your voice.

🔧 Features
🎤 Listens to your voice commands using the microphone.

🧠 Recognizes spoken commands with Google Speech Recognition.

🚀 Opens apps like:

Notepad

Calculator

Google Chrome

🌐 Performs a web search if the command doesn't match any known app.

🗣️ Responds using text-to-speech feedback.

📁 Project Structure
main.py – Core script that runs the assistant.

▶️ Getting Started
Requirements
Python 3.x

Microphone connected to your device

Install Dependencies
bash
Copy
Edit
pip install speechrecognition pyttsx3 pyaudio
💡 If you face issues installing pyaudio, try:

On Windows: pip install pipwin && pipwin install pyaudio

On Linux: sudo apt install portaudio19-dev python3-pyaudio

Run the Assistant
bash
Copy
Edit
python main.py
🛠️ How It Works
The program prompts you to speak.

It converts your speech to text using Google’s API.

If the spoken text matches a known app, it launches the app.

Otherwise, it opens a Google search for your query.

📝 Customization
To add more apps, edit the apps dictionary in main.py:

python
Copy
Edit
apps = {
    "notepad": "notepad.exe",
    "calculator": "calc.exe",
    "chrome": "C:\\Program Files\\Google\\Chrome\\Application\\chrome.exe",
    "your_app": "path\\to\\your_app.exe"
}
❗ Limitations
Requires an active internet connection for speech recognition.

Basic app matching (based on keyword presence).

No wake word detection or continuous listening (single-command based).

📄 License
This project is open for personal and educational use.

