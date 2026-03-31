# Vincent Mwebi — Portfolio Site

Personal portfolio built with **Flask**. Single-page site with tabbed sections (About, Experience, Projects & skills), contact links, and a downloadable résumé PDF.

## Run locally

**Requirements:** Python 3.10+ (or similar)

```bash
pip install flask
python app.py
```

Open **http://127.0.0.1:5000/** in your browser.

> For reproducible installs you can use `pip install -r requirements.txt` if you add a `requirements.txt` (e.g. `flask==3.0.0`).

## Project layout

| Path | Purpose |
|------|--------|
| `app.py` | Flask app; `/` renders the portfolio template |
| `templates/portfolio.html` | HTML, CSS, tab UI, and content |
| `static/` | Static files (e.g. `Vincent_Mwebi_Resume.pdf`) |

## Résumé PDF

Place your PDF in `static/` as **`Vincent_Mwebi_Resume.pdf`** so the “Download PDF” link works. The filename must match what `portfolio.html` uses in `url_for('static', filename='...')`.

## Links (from the site)

- **Email:** Mosesmwebi@gmail.com  
- **LinkedIn:** https://www.linkedin.com/in/vincent-mwebi-375914158/  
- **GitHub:** https://github.com/mosesmw  

## Production note

`app.run(debug=True)` is for **local development** only. For deployment, use a production WSGI server and turn debug off (follow your host’s Flask/Python guide).
