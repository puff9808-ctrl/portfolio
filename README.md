# Bhukya Gowtham Naik — Personal Portfolio

A responsive portfolio built with **HTML, CSS, and vanilla JavaScript**, with an animated portrait, scroll reveals, mobile navigation, project details, résumé links, and contact links.

## Run locally on Windows

### Option 1: Open directly
1. Open the portfolio folder.
3. Double-click `index.html`. It opens in your default browser.

### Option 2: Run a local server (recommended)
If Python is installed:
1. Open the project folder in File Explorer.
2. Click the address bar, type `cmd`, and press Enter.
3. Run:

```bat
python -m http.server 5500
```

4. Open http://localhost:5500 in your browser.
5. Stop the server with `Ctrl+C`.

No npm install, build step, API key, or backend is required. Google Fonts loads from the internet; system fonts are used if offline.

## Portfolio links

The résumé and portrait are stored locally in `assets/`. Project cards link to the PDF Summarizer and AI Resume Checker repositories; the resume checker card also links to its live demo.

## Deploy to Vercel

Set the Vercel project **Root Directory** to the folder containing `index.html` and the `assets/` directory (`portfolio-main/` in this repository). Make sure `assets/gowtham-portrait.jpg` is committed and included in the deployment. The portrait uses a root-relative URL, so it is served from `/assets/gowtham-portrait.jpg`.

## Project structure

```text
portfolio-main/
├── index.html
├── style.css
├── effects.css
├── script.js
├── README.md
└── assets/
    ├── gowtham-portrait.jpg
    └── resume.pdf
```

## Upload to GitHub

Create an empty repository, then run these commands from this folder:

```bat
git init
git add .
git commit -m "Add personal portfolio website"
git branch -M main
git remote add origin https://github.com/YOUR-GITHUB-USERNAME/portfolio.git
git push -u origin main
```

Replace the repository URL with your actual GitHub repository URL. For future changes, use `git add .`, `git commit -m "Describe your changes"`, and `git push`.
