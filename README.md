# LangChain + Gemini Translator (Streamlit)

A minimal Streamlit app that demonstrates using LangChain with Google's Gemini model to translate text between languages.

## What it is

- Single-file demo: `gemini_applanguage_translator.py`
- Uses `langchain_core` + `langchain_google_genai` to call Gemini (Gemini Flash).

## Prerequisites

- Python 3.10+ recommended
- Git (optional)

## Setup

1. Create a virtual environment and activate it:

   PowerShell

   ```powershell
   python -m venv myvenv
   .\myvenv\Scripts\Activate.ps1
   ```

   Command Prompt

   ```batch
   python -m venv myvenv
   myvenv\Scripts\activate.bat
   ```

2. Install dependencies:

   If you have a `requirements.txt`: `pip install -r requirements.txt`

   Example (install minimal runtime packages):

   ```bash
   pip install streamlit python-dotenv langchain-core langchain-google-genai google-genai
   ```

3. Configure credentials / environment variables:
   - Create a `.env` file or set environment variables as required by your Google/GenAI auth method.
   - The app calls `load_dotenv()` so a `.env` file in the project root will be read automatically.

## Run the app

```bash
streamlit run gemini_applanguage_translator.py
```

Open the URL printed by Streamlit (usually `http://localhost:8501`).

## Notes

- A `.gitignore` is included to ignore virtual environments, caches, and common artifacts.
- If you need to pin exact versions, create a `requirements.txt` from your working environment.

## Files

- `gemini_applanguage_translator.py` — main demo app
- `.gitignore` — generated ignore rules
- `README.md` — this file
