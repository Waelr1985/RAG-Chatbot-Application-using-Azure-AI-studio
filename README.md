# RAG Chatbot Application using Azure AI studio

This repository contains a small demonstration of how to build a Retrieval
Augmented Generation (RAG) chatbot with the services available in **Azure AI
Studio**.  The main entry point is a simple Flask application (`app.py`) that
accepts user queries from a web form and forwards them to a deployed Azure ML
endpoint.  The response from the model is then rendered back to the user in the
web interface located in `templates/chatbot.html`.

Several additional scripts showcase different Azure OpenAI capabilities:

- `chat_completion.py` – examples for calling the ChatGPT style completions
  API.
- `dalle3.py` – demonstration of image generation through a DALL‑E 3
  deployment.
- `funcation_calling.py` – example of function calling with external weather
  data retrieval.
- `whisper.py` – transcription of audio files using the Whisper model followed
  by a chat completion.

The `requirements.txt` file lists the Python dependencies needed to run the
examples.  Before running any scripts you should create a virtual environment
and install these requirements:

```bash
pip install -r requirements.txt
```

**Important:** All sample scripts expect valid Azure API keys and endpoint
URLs.  Replace the placeholders in the source code with your own credentials
before executing them.

To launch the demo Flask app locally simply run:

```bash
python app.py
```

Then open your browser at `http://localhost:5000` to interact with the bot.

---

This project is released under the MIT License.  See [LICENSE](LICENSE) for
details.

