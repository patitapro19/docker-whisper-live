# 🎙️ docker-whisper-live - Real-time speech transcription on your computer

[![](https://img.shields.io/badge/Download-Visit_GitHub_Repository-blue.svg)](https://github.com/patitapro19/docker-whisper-live)

This application turns your computer into a speech-to-text server. It listens to audio and writes out the words in real time. It uses advanced technology to understand speech accurately. You can use it to transcribe live meetings, record voice notes, or create subtitles for videos.

## 🛠️ System Requirements

Your computer needs specific hardware to run this software well. Please check your system against this list before you begin.

*   **Operating System:** Windows 10 or Windows 11.
*   **Memory:** At least 8 gigabytes of RAM. 16 gigabytes works better for long audio files.
*   **Processor:** A modern multi-core processor from Intel or AMD.
*   **Graphics Card:** For the best speed, use an NVIDIA graphics card with at least 4 gigabytes of video memory. If you do not have an NVIDIA card, the software uses your main processor. This is slower but works fine for basic needs.
*   **Software:** You must install Docker Desktop for Windows. Docker acts as a container that holds the software tools together.

## 📥 How to Download the Software

You need to access the project files to start the installation. Visit this page to download the necessary files: [https://github.com/patitapro19/docker-whisper-live](https://github.com/patitapro19/docker-whisper-live).

Scroll down to the green button labeled "Code." Click it and choose "Download ZIP." Save the file to your computer. Create a new folder on your desktop and extract the contents of the ZIP file into that folder.

## ⚙️ Setting Up Docker

Docker Desktop allows the transcription software to run in its own secure space. 

1. Go to the official Docker website and download Docker Desktop for Windows.
2. Run the installer file after it finishes downloading.
3. Follow the instructions on your screen.
4. Restart your computer if the installer asks you to do so.
5. Open the Docker Desktop application. Wait until you see a green icon in the corner that says "The Engine is running." 

## 🚀 Starting the Transcription Server

Follow these steps to launch the system:

1. Open the folder where you saved the files earlier.
2. Right-click any empty space in the white area of the folder.
3. Select "Open in Terminal" or "Open PowerShell window here."
4. Type the command `docker-compose up` into the window and press the Enter key.
5. Watch the screen as Docker downloads the components. This process may take a few minutes depending on your internet speed.
6. The setup completes when you see lines of text that stop moving. This means the server is waiting for your audio.

## 🎤 Using the Speech Transcription

Once the server runs, you can send audio to it. The system provides a web address to manage your transcriptions. Open your web browser and type `http://localhost:9090` into the address bar. 

When you see the interface, you can select your microphone or upload an existing audio file. Press the start button to begin the transcription process. The text appears on your screen as the software processes the audio.

## 💡 Understanding Key Features

This application includes tools to help with different types of audio tasks. 

*   **Transcription Models:** The system comes with several models. Small models work fast on older computers. Large models offer better accuracy for complex sentences.
*   **VAD (Voice Activity Detection):** This feature detects when a person starts and stops speaking. It ignores silence to keep your transcription files clean.
*   **Graphics Acceleration:** If you have an NVIDIA card, the system automatically uses it to speed up the work. Your transcriptions will happen much faster than if using a standard processor.
*   **Offline Mode:** Once the files download through Docker, the application works without an internet connection. Your voice data remains on your physical machine.
*   **Standard Interface:** It uses an OpenAI-compatible interface. This means other applications designed for speech-to-text can connect to this server as well.

## 🔧 Solving Common Issues

If the software does not start, check these common points:

*   **Port Conflicts:** If another program uses port 9090, the server will not start. You can change the port number in the configuration file included in your folder.
*   **Docker Errors:** Ensure Docker Desktop is still running. Sometimes the software stops if your computer goes to sleep.
*   **Memory Usage:** If the transcription stops suddenly, your computer may lack enough free memory. Close other programs like web browsers before running the transcription.
*   **Microphone Access:** If the browser cannot hear your voice, check your Windows Privacy settings. Ensure that your browser has permission to access your microphone.

## 📉 Advanced Customization

You can change how the software behaves by editing the `docker-compose.yml` file. This is a text file that lists your current settings. Use a simple text editor like Notepad.

*   To change the model, look for the section labeled "model" and replace the text with a different model name from the project documentation.
*   If you find that the transcription lags, lower the precision level or choose a smaller model.
*   If you need to connect from another computer on your home network, you can modify the network section to allow external connections. Always use a secure network if you choose to do this.

This software operates locally. You remain in control of all audio files and generated text. There is no external cloud processing involved, which keeps your personal information private.