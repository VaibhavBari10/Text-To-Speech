
# Text-to-Speech Application

A Python desktop application that converts written text into spoken audio. It provides a graphical interface for reading typed text or PDF content aloud, selecting a voice, adjusting speech speed, and saving generated speech as an MP3 file. The project also includes speech input and text translation functionality.

## Features

- **Text-to-Speech:** Read text entered in the application aloud.
- **PDF-to-Speech:** Select a PDF and convert its extracted text into speech.
- **Voice Selection:** Choose between the available male and female system voices.
- **Speech Speed Control:** Adjust the rate at which text is spoken.
- **MP3 Export:** Save generated speech as an audio file.
- **Speech Recognition:** Capture speech through a microphone and convert it to text.
- **Translation:** Translate text using `googletrans`.
- **Desktop GUI:** Built with Python's Tkinter and ttk widgets.

> **Note:** Available voices and language support depend on the voices installed on your computer and the translation/speech services used by the application.

## Technology Stack

- **Python**
- **Tkinter / ttk** — desktop graphical interface
- **pyttsx3** — text-to-speech using locally available speech engines
- **SpeechRecognition** — microphone input and speech recognition
- **PyPDF2** — PDF text extraction
- **googletrans** — text translation
- **gTTS** — Google Text-to-Speech support
- **playsound** — audio playback

## Project Structure

```text
Text-To-Speech/
├── Images/                 # Project images/assets
├── main.py                 # Main text-to-speech application
├── loginsystem.py          # Login interface/system
├── requirement.txt         # Python dependencies
├── welcome1.mp3            # Welcome audio file
├── datasheet.txt           # Project/system information
└── datasheet-LAPTOP-7DCNI5Q9.txt
```

## Prerequisites

- Windows is recommended for the current desktop application.
- Python 3 installed and added to PATH.
- A working microphone for speech recognition.
- Speakers or headphones for audio playback.
- Internet access for Google-based speech recognition, translation, or gTTS features.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/VaibhavBari10/Text-To-Speech.git
   cd Text-To-Speech
   ```

2. (Recommended) Create and activate a virtual environment:

   ```bash
   python -m venv .venv
   ```

   On Windows Command Prompt:

   ```bat
   .venv\Scripts\activate
   ```

   On Windows PowerShell:

   ```powershell
   .\.venv\Scripts\Activate.ps1
   ```

3. Install the dependencies:

   ```bash
   python -m pip install --upgrade pip
   pip install -r requirement.txt
   ```

4. Start the application:

   ```bash
   python main.py
   ```

   If you need to open the login screen first, run:

   ```bash
   python loginsystem.py
   ```

   Use the entry point that matches your intended workflow. The repository currently contains both scripts.

## How to Use

1. Launch the application.
2. Choose the text input option and type or paste the text you want to hear, or select the PDF option and upload a PDF file.
3. Select an available voice.
4. Adjust the speech rate using the application's speed control.
5. Use the speak/play action to listen to the generated speech.
6. Use the download/save option to choose a folder and save the audio output.
7. For speech input, allow microphone access and speak clearly when prompted.
8. Use the translation controls to translate text into the selected target language, where supported.

## Troubleshooting

- **No voice is available:** Check your operating system's speech settings and install a supported voice.
- **Microphone errors:** Check Windows microphone permissions and confirm that the correct recording device is enabled.
- **Dependency installation errors:** Confirm that the virtual environment is active, then reinstall from `requirement.txt`.
- **Translation or online recognition fails:** Check your internet connection and the service availability.
- **PDF text is missing or garbled:** Some PDFs are scanned images rather than selectable text. Such files may require OCR before their contents can be extracted.
- **Audio does not play:** Check the selected output device and verify that the required audio playback packages are installed.

## Limitations

- Speech quality and available voices depend on the installed speech engine and voice packages.
- Google-backed recognition, translation, and gTTS features may require an internet connection.
- PDF extraction works best with text-based PDFs; scanned documents may not produce usable text without OCR.
- The exact behavior of the login workflow depends on the configuration in `loginsystem.py`.

## Future Improvements

- Add support for more languages and configurable voice options.
- Improve PDF handling for multi-page documents and scanned PDFs using OCR.
- Add clearer error messages and input validation.
- Modernize dependency versions and document tested Python versions.
- Add screenshots and automated tests.

## Contributing

Contributions and suggestions are welcome. You can open an issue to report a problem or submit a pull request with an improvement.

## Author

**Vaibhav Bari**

- GitHub: [VaibhavBari10](https://github.com/VaibhavBari10)

## License

No license file was visible in the repository when this README was prepared. Add a `LICENSE` file and update this section if you intend to publish the project under a specific open-source license.
