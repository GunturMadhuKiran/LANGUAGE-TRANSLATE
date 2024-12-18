Voice-to-Text Translation Application

This project is a Python-based application that captures voice input, recognizes the spoken text, detects its language, translates it into a target language, and generates an audio file in the translated language.

Features

Captures voice input using the microphone.

Recognizes spoken text using Google Speech Recognition.

Detects the language of the recognized text.

Translates the recognized text into a user-specified target language.

Converts the translated text into an audio file using Google Text-to-Speech (gTTS).

Prerequisites

Ensure you have the following installed:

Python 3.7 or higher

Required Python libraries (install via pip):

speech_recognition

googletrans==4.0.0-rc1

gtts

Installation

Clone this repository:

Install the required libraries:

pip install -r requirements.txt

Ensure your microphone is working and accessible.

Usage

Run the script:

python app.py

When prompted, enter the target language (e.g., Hindi, Telugu, Tamil).

Speak into the microphone when instructed. The application will:

Recognize your speech.

Detect the language of the recognized text.

Translate the text into the specified target language.

Save the translated audio to an outputs folder.

The translated audio will automatically play if your system supports the playback command.

Supported Languages

The application currently supports translation to the following languages:

Hindi (hi)

Telugu (te)

Kannada (kn)

Tamil (ta)

Malayalam (ml)

Bengali (bn)

File Structure

voice-to-text-translation/
|-- app.py              # Main application script
|-- requirements.txt    # Required libraries
|-- outputs/            # Directory where translated audio files are saved

Requirements File

Create a requirements.txt file with the following content:

speech_recognition
googletrans==4.0.0-rc1
gtts

Notes

The googletrans library may experience occasional issues with translations. If translation fails, check your network connection or try again later.

Ensure that the outputs directory exists or will be created during the script execution.
