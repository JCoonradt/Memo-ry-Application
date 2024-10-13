# Memo-ry: Empowering Independence for People with Dementia

Memo-ry is an innovative web-based application designed to support individuals with dementia by recording and processing audio from daily conversations. 
It listens for tasks, demands, or instructions and automatically generates an organized to-do list based on the recognized tasks. 
By simplifying the task-tracking process, Memo-ry helps individuals maintain their independence, reduce confusion, and make it easier to manage day-to-day responsibilities.

## Features

- **Speech-to-Text Recognition**: Real-time transcription of spoken words into text using the browser's built-in speech recognition.
- **Task Extraction**: Automatically extracts tasks from the transcription and displays them in a checklist format.
- **Checklist with Task Completion**: Each extracted task is displayed with a checkbox, allowing users to mark tasks as completed.
- **Simple UI**: Clean and easy-to-use interface with buttons to start and stop recordings.

## Getting Started

### Prerequisites

- A modern web browser with support for the Web Speech API (Chrome and Edge support this feature).
- Internet connection (for task extraction via the Cerebras API).
- **Cerebras API Key**: You will need to sign up for the Cerebras API and get your own API key for the task extraction functionality.

### Installation

1. Clone or download this repository to your local machine.

   ```bash
   git clone https://github.com/your-username/memo-ry.git
   cd memo-ry
   
2. Open the index.html file in your web browser.
3. API Key Setup: Memo-ry uses the Cerebras API to extract tasks from the transcribed text. You must replace the placeholder API key with your own for the task extraction to work.
  -Sign up for an API key at [Cerebras]([url](https://cloud.cerebras.ai/)).
  -Replace the API key in the code:
   In the extractTasks function in index.html, find this line:
      ```
      const token = 'YOUR_API_KEY';  // Replace with your actual API key
Replace 'YOUR_API_KEY' with your actual API key.


### Usage
1. Start Recording: Click the Start Recording button to begin recording audio.
2. Speak: Speak clearly into your device’s microphone. The app will transcribe your speech in real-time.
3. Stop Recording: Once finished, click the Stop Recording button.
4. Extracted Tasks: The app will automatically extract tasks from the transcription and display them as a checklist.
5. Complete Tasks: You can mark tasks as complete by clicking the checkboxes next to each task.
6. API Integration (IMPORTANT). Memo-ry uses the Cerebras API to extract tasks from the transcribed text.
To use this app, you must replace the placeholder API key with your own.


Project Structure
bash
Copy code
.
├── index.html          # Main HTML file containing the UI and JavaScript logic
└── README.md           # Project documentation

### Technology Stack
HTML/CSS/JavaScript: The front-end of the application.
SpeechRecognition API: Used for speech-to-text transcription.
Cerebras API: Handles task extraction from transcriptions.

### Known Issues
The Web Speech API is only supported in certain browsers, primarily Google Chrome and Microsoft Edge.
Requires an active internet connection for task extraction functionality.
