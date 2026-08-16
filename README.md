# ABC Alphabet Explorer — Streamlit

A local Streamlit version of the ABC Alphabet Explorer.

## Windows / PyCharm

```powershell
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
streamlit run app.py
```

Then open the local URL Streamlit prints, normally:
http://localhost:8501

## Notes

- The SQLite database remains in `db/alphabet.db`.
- Word illustrations remain local under `db/images/A` through `db/images/Z`.
- Letter-specific landscapes remain under `static/landscapes`.
- Background music is local at `db/kids_attention_music.wav`.
- Images, landscapes and audio are embedded into the browser component at runtime so the app does not depend on external URLs.
- Speech uses the browser's Speech Synthesis API and prefers `en-IN` (Indian English) when the browser/OS provides it.
- Background music starts only after the user clicks the music toggle, due to normal browser autoplay restrictions.
