# AI Music Assistant

## Overview
AI Music Assistant is an intelligent voice-controlled application that helps users find and play music. It utilizes speech recognition, natural language processing, and web automation to search for songs on YouTube and play music from the local system.

## Features
- **Voice Commands**: Users can interact with the assistant using voice commands.
- **Music Search**: Searches for songs on YouTube based on user input.
- **YouTube Song Retrieval**: Fetches accurate song links from YouTube.
- **Text-to-Speech (TTS)**: Provides voice responses using gTTS.
- **Automated Web Browsing**: Uses Selenium WebDriver to open YouTube links.
- **Streamlit UI**: Provides a simple UI for user interaction.

## Tech Stack
- **Programming Language**: Python
- **Libraries Used**:
  - `speech_recognition`: Converts spoken language into text.
  - `pyttsx3` & `gtts`: Converts text to speech.
  - `selenium`: Automates web interactions.
  - `streamlit`: Provides a user-friendly interface.
  - `googleapiclient`: Fetches YouTube search results.
  - `langchain_groq`: Uses AI models to generate relevant song links.
  - `dotenv`: Loads environment variables securely.

## Installation
### Prerequisites
- Python 3.8+
- Google Chrome (for Selenium WebDriver)
- Required API keys:
  - **Groq API Key**: For language processing.
  - **YouTube API Key**: For fetching search results.

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/ai-music-assistant.git
   cd ai-music-assistant
   ```
2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Set up environment variables:
   - Create a `.env` file in the root directory and add:
     ```
     GROQ_API_KEY=your_groq_api_key
     YOU_API_KEY=your_youtube_api_key
     ```
5. Install Selenium WebDriver:
   - Download the appropriate **ChromeDriver** for your Chrome version from [ChromeDriver](https://chromedriver.chromium.org/downloads)
   - Extract and place it in the project directory or set it in the system path.

## Usage
### Running the Application
Run the assistant using:
```bash
python main.py
```

### Commands
- **Play music**: Plays local music files.
- **Search [song name] on YouTube**: Finds and plays a song on YouTube.
- **Stop**: Closes the YouTube player.
- **Exit**: Terminates the assistant.

### Using Streamlit UI
To launch the web interface:
```bash
streamlit run main.py
```

## Troubleshooting
- **Speech recognition not working**:
  - Ensure your microphone is enabled and accessible.
  - Try running the script with administrator privileges.
- **YouTube search not working**:
  - Check if the YouTube API key is valid and has enough quota.
- **WebDriver issues**:
  - Ensure `chromedriver` matches your Chrome version.

## Contact
For any queries, contact **Rithwik** at: [rithwik.t2003@gmail.com](mailto:rithwik.t2003@gmail.com)



