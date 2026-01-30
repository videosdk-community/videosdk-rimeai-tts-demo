# VideoSDK X RimeAI TTS Demo

This example demonstrates how to build a conversational AI Voice Agent using VideoSDK's Cascading Pipeline with [**RimeAI TTS**](https://pypi.org/project/videosdk-plugins-rime/).

# Architecture Overview

The agent is built using VideoSDK’s Cascading Pipeline, where each component operates continuously instead of sequential batch processing.
<img width="3026" height="582" alt="videosdk_casading_pipeline" src="https://github.com/user-attachments/assets/cbdb6a40-efb4-41e9-b056-868b0f9ba287" />

## Prerequisites

- Python 3.11+
- A [VideoSDK Account](https://dub.sh/A1vscPp)
- A [RimeAI API Key](https://rime.ai/)
- A [Deepgram API Key](https://console.deepgram.com/apikeys)
- A [Google Gemini API Key](https://aistudio.google.com/apikey)

## Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/videosdk-community/videosdk-rimeai-tts-demo.git
    ```

2.  **Create a virtual environment:**

    ```bash
    python -m venv .venv
    ```

    Activate the virtual environment:
    - MacOS/Linux: `source .venv/bin/activate`
    - Windows: `.venv\Scripts\activate`

3.  Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

4.  Set up environment variables:
    Copy `.env.example` to `.env` and fill in your keys.

    ```bash
    cp .env.example .env
    ```

    **Required Variables:**
    - `RIME_API_KEY`
    - `DEEPGRAM_API_KEY`
    - `GOOGLE_API_KEY`
    - `VIDEOSDK_AUTH_TOKEN`

## Usage

Run the agent with the following command:

```bash
python main.py
```

## What Happens Next?

The agent creates a VideoSDK playground session and a joinable URL is printed in the terminal, Open the URL in your browser and Start speaking the agent will respond in real time 🎙️

<img width="1459" height="815" alt="Screenshot 2026-01-29 at 12 03 20 PM" src="https://github.com/user-attachments/assets/0b6e20eb-7d84-404e-bdea-ad97757a8230" />

## Documentation

- [RimeAI TTS Plugin Documentation](https://docs.videosdk.live/ai_agents/plugins/tts/rime-tts)
- [Cascading Pipeline Documentation](https://docs.videosdk.live/ai_agents/core-components/cascading-pipeline)
