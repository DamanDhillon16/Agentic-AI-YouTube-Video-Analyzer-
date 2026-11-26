# YouTube Video Analyzer Agent (Agno + Groq + Streamlit)

## Demo
[Watch the 36-Second Screen Recording](demo.md)

An agentic AI application built with **Agno** and **Groq** (`openai/gpt-oss-120b`), paired with a **Streamlit** web interface (`ui.py`). Paste any YouTube video URL into the app, and the agent fetches metadata and captions using `YouTubeTools` to produce a structured video overview, timestamped segments, key learning points, and content references.

## How It Works

1. **Enter a YouTube URL:** Open the Streamlit interface and paste a YouTube video link.
2. **Fetch Video Data & Captions:** The Agno agent calls `YouTubeTools` to retrieve video metadata and transcript segments.
3. **Generate Structured Analysis:** The model (`openai/gpt-oss-120b` via Groq) organizes the content into an overview, content-type cues, timestamped breakdown (`[start_time, end_time, detailed_summary]`), key takeaways, and practical references.
4. **Review in the UI:** Read the formatted Markdown breakdown directly in your browser.

## Features

- **Transcript & Metadata Extraction:** Uses Agno's `YouTubeTools` to pull video details and captions from YouTube URLs.
- **Structured Video Breakdown:** Organizes output into a video overview, content-type emojis/cues, timestamped segments, key takeaways, and references.
- **Interactive Streamlit UI:** Provides a browser-based interface (`ui.py`) for entering YouTube links and viewing formatted responses.
- **Environment-Based Configuration:** Loads API keys securely via `python-dotenv` without hardcoding secrets.

## Project Structure

├── agent.py            # Agno agent definition, model setup, tools, and instructions
├── ui.py               # Streamlit user interface
├── requirements.txt    # Python dependencies
├── .gitignore          # Ignored secrets, cache, and environment files
└── README.md           # Project documentation

Daman Dhillon |
[LinkedIn](https://https://www.linkedin.com/in/daman-jeet-kaur-dhillon-324191312/) | [GitHub](https://github.com/DamanDhillon16)
