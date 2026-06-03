# VG Interior Design Website

A bilingual (English/Chinese) Flask website for VG Interior Design, Sydney.

## Project Structure

```
vg-archi/
├── app.py
├── requirements.txt
├── render.yaml
├── templates/
│   └── index.html
└── static/
    └── images/
        ├── Vector Graphic logo.png
        ├── Bedroom 2 - 1.png
        ├── Kitchen 6 -5.png
        ├── Laundry 10.png
        ├── Main Bed  19.png
        ├── Master Ens 03.png
        ├── New Bath 5.png
        ├── new Ground Ensuite 02.png
        ├── Office 2.png
        ├── Powder Room 5.png
        ├── Public L520.png
        ├── Spare Room 14.png
        └── Wardrobe 1.png
```

## Local Setup

```bash
pip install -r requirements.txt
python app.py
```
Then open http://localhost:5000

## Deploy to Render

1. Push this project to a **GitHub** repository
2. Go to https://render.com → New → Web Service
3. Connect your GitHub repo
4. Render auto-detects `render.yaml` — click **Deploy**
5. Your site will be live at `https://vg-archi.onrender.com` (or your custom name)

### Manual Render settings (if not using render.yaml):
- **Environment**: Python
- **Build Command**: `pip install -r requirements.txt`
- **Start Command**: `gunicorn app:app`

## Adding Images

Place all images from the `static` folder into `static/images/`.
The exact filenames must match what's in the screenshots (spaces and case-sensitive).
