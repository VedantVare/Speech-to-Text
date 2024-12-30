# Speech Recognition and Text-to-Speech Program

This project is a Python-based program that:
1. Listens to your voice using a microphone.
2. Converts spoken words into text.
3. Allows interaction via voice commands.

## Features
- **Speech Recognition**: Captures and understands your voice input.
- **Text-to-Speech**: Responds using a natural-sounding voice.
- **Continuous Listening**: Keeps running until stopped manually.

## Requirements
- Python 3.7 or higher
- Libraries:
  - `pyttsx3`: For text-to-speech functionality.
  - `speech_recognition`: For recognizing spoken words.

Install the required libraries:
```bash
pip install pyttsx3 SpeechRecognition
```

## How It Works
1. The program uses the `speech_recognition` library to listen to audio input from your microphone.
2. Converts the audio into text using Google’s speech recognition API.
3. Responds or processes commands based on the spoken input.

## Usage
1. Run the script:
   ```bash
   python speech_recognition_tts.py
   ```
2. Speak into the microphone. The program will:
   - Print what you said as text.
   - Ask you to repeat if it doesn’t understand.
3. The loop continues until you manually stop it.

## Settings
- **Voice Settings**: Configurable through `pyttsx3` (e.g., voice type, rate of speech).
- **Thresholds**:
  - `pause_threshold`: Controls how long the program waits for a pause in speech.
  - `energy_threshold`: Sets the microphone sensitivity to ambient noise.

## Notes
- Ensure your microphone is properly configured and working.
- Speak clearly for better recognition.
- Modify the speech rate or voice settings in the code if needed:
  ```python
  engine.setProperty("rate", 150)  # Adjusts the speed of speech
  engine.setProperty("voice", voices[1].id)  # Changes the voice
  ```

## License
This project is open-source and can be used or modified for learning or personal projects.
