# Meeting-Summary 

## Overview

The **Meeting Summary** is a tool designed to streamline the process of extracting and summarizing key points from meetings. By providing a video file of your meeting, the tool automatically extracts the audio, converts it into text, and then generates a concise meeting agenda based on the content of the discussion.

## Features

- **Video to Audio Extraction**: Upload a video file of your meeting, and the tool will extract the audio using the Whisper model.
- **Speech-to-Text Conversion**: The extracted audio is converted into text, capturing all spoken content from the meeting.
- **Automated Meeting Agenda Generation**: Using OpenAI's capabilities, the tool analyzes the transcribed text and generates a structured meeting agenda that highlights the key points and decisions made during the meeting.

## How It Works

1. **Upload Video**: Start by uploading a video file of your meeting.
2. **Audio Extraction**: The tool extracts the audio from the uploaded video.
3. **Text Conversion**: The extracted audio is then converted into text using Whisper, ensuring accurate transcription of the spoken content.
4. **Agenda Generation**: OpenAI processes the transcribed text and generates a meeting agenda based on the content. The agenda will include key points, decisions, and action items discussed during the meeting.
5. **Download Agenda**: Once the agenda is generated, you can download it in a readable format.

## Requirements

- Python 3.7 or later
- OpenAI API key
- Whisper model for speech-to-text conversion
- Video files in supported formats (e.g., .mp4, .mov)

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/meeting-summary.git
   cd meeting-summary
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Set up your OpenAI API key:

   ```bash
   export OPENAI_API_KEY='your-openai-api-key'
   ```

## Usage

1. Place your video file in the `input` directory.
2. Run the main script:

   ```bash
   python main.py --input ./input/your-meeting-video.mp4 --output ./output/meeting-agenda.txt
   ```

3. The tool will extract the audio, convert it to text, generate the agenda, and save the result in the specified output file.


