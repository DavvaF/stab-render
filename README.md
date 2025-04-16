# AI-baserad Videostabilisering – Streamlit App för Render

Detta är en webbaserad app för att stabilisera skakigt videomaterial (.mp4 och .mov) med hjälp av AI (VidStab + OpenCV).

## 🚀 Så här kör du appen på [Render.com](https://render.com)

### 1. Skapa ett nytt GitHub-repo
Ladda upp hela innehållet från denna ZIP till ett nytt repo.

### 2. Skapa en Web Service i Render
1. Gå till dashboard.render.com
2. Klicka på **"New +" → "Web Service"**
3. Välj ditt repo
4. Render läser automatiskt `render.yaml`

### 3. Ändra "Start Command"
Render försöker använda `gunicorn`. Ändra till:

```bash
streamlit run app.py
```

### 4. Klart! 🎉
Appen startar automatiskt. Du kan ladda upp videofiler upp till **500 MB**.

---

## 📁 Viktiga filer

- `render.yaml` – konfigurerar Render
- `.streamlit/config.toml` – sätter maxUploadSize och port
- `requirements.txt` – installerar alla beroenden
- `app.py` – själva Streamlit-appen
