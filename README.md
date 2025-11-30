# Interactive AI Chatbot

This workspace contains a minimal interactive AI chatbot with two web UI options:

- Streamlit app: `streamlit_app.py` (recommended)
- Flask app: `app_flask.py` (optional)

Features
- Uses OpenAI if `OPENAI_API_KEY` is set in the environment; otherwise falls back to a simple echo.

Running locally (PowerShell)

1. Create a virtual environment and install requirements

```powershell
python -m venv .venv; .\.venv\Scripts\Activate.ps1; pip install -r requirements.txt
```

2. Run Streamlit app

```powershell
streamlit run streamlit_app.py
```

3. Or run Flask app

```powershell
python app_flask.py
```

Deployment notes
- Streamlit Cloud: push to a GitHub repo and connect to Streamlit Cloud.
- Docker: create a small Dockerfile that installs requirements and runs `streamlit run`.

Environment
- To enable OpenAI responses, set `OPENAI_API_KEY` in your environment before running.

