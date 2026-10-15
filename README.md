# EduAI Quiz

Streamlit-based AI quiz application.

## Run locally

```bash
python -m pip install -r requirements.txt
python -m streamlit run EduAIQuiz_app.py
```

For local development, create a `.env` file containing `GEMINI_API_KEY=your_key`. Never commit `.env`.

## Deploy to Streamlit Community Cloud

1. Push this repository to GitHub.
2. Create an app at https://share.streamlit.io/ with entrypoint `EduAIQuiz_app.py`.
3. In Advanced settings / Secrets, add:

```toml
GEMINI_API_KEY = "your_key"
```

Do not commit `.env`, student results, or private PDF materials. Community Cloud does not guarantee persistence of local file storage; use a database or cloud storage for durable shared materials and results.
