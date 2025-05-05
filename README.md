# Cerita dari Suara

A simple web application to convert voice recordings into text-based stories using OpenAI's Whisper speech recognition model.

## Features
- Upload `.mp3`, `.wav`, or other supported audio files
- Transcribe audio into text using Whisper
- Display the story/monologue on a webpage

## Requirements
- Python 3.8+
- Flask
- OpenAI Whisper

## Setup
```bash
# Clone the repository
git clone https://github.com/your-username/cerita-dari-suara.git
cd cerita-dari-suara

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

# Install dependencies
pip install -r requirements.txt

# Run the app
python app.py
```

Then open your browser and go to `http://127.0.0.1:5000/`

## Folder Structure
```
.
├── app.py              # Main Flask application
├── templates/
│   └── index.html      # Upload form & result page
├── static/             # (Optional) Styling assets
├── uploads/            # Stores uploaded audio files
├── requirements.txt    # Python dependencies
└── README.md           # This file
```

## Notes
- This uses the base Whisper model. You can change it to `tiny`, `small`, `medium`, or `large` depending on accuracy/speed tradeoffs.
- For deployment, disable `debug=True` and consider using a production server like Gunicorn.

---

Made with ❤️ for your journey of storytelling from sound.
