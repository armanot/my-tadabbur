# my-tadabbur

my-tadabbur/
├── backend/
│   ├── app/
│   │   ├── __init__.py
│   │   ├── routes.py              # Flask routes (API)
│   │   └── utils.py               # Utility functions (search, text ops)
│   ├── data/
│   │   └── quran.json             # Quran dataset (static or imported)
│   ├── venv/                      # Your Python virtual environment (myt-venv)
│   ├── requirements.txt           # Python dependencies
│   └── run.py                     # Flask app entry point
│
├── frontend/
│   ├── public/
│   │   └── index.html             # Base HTML file
│   ├── src/
│   │   ├── assets/
│   │   │   ├── css/
│   │   │   │   └── styles.css
│   │   │   └── images/
│   │   ├── js/
│   │   │   └── main.js            # Main JS logic (Tadabbur rendering, API calls)
│   │   └── components/            # Optional: modular JS components
│   ├── package.json               # npm dependencies
│   ├── vite.config.js             # If using Vite (optional)
│   └── README.md
│
├── .gitignore
├── README.md
└── .env                           # Configs like Flask API URL


frontend/
├── index.html                  # Main UI: Lists Surahs, Verses
├── tadabbur.html               # Reflection view for selected verse
├── assets/
│   ├── css/
│   │   └── styles.css          # All styles go here
│   └── js/
│       ├── main.js             # Handles data fetch, navigation
│       ├── api.js              # JS for calling backend endpoints
│       └── utils.js            # Optional helpers (e.g. sanitization)
├── images/                     # Any logos, icons, etc.
└── README.md















# Prepare backend
cd backend
python -m venv myt-venv
source myt-venv/bin/activate
pip install flask
pip freeze > requirements.txt

# prepare frontend
cd frontend
npm init -y
