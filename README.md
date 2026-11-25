# CV Studio

A single-file web app to edit a CV with a live A4 preview, built-in quality checks and print-to-PDF.
No build step, no dependencies. Open `index.html` in a browser.

## Features
- Edit profile, jobs, skills, languages, certifications and education
- Live preview that matches the print layout
- Checks panel: typos, duplicate skills, thin bullets, placeholders, long summary, vague Dutch level
- Autosave in the browser (localStorage) and a JSON backup box
- Print / Save as PDF (A4)

## Run
Open `index.html`, or serve the folder: `python3 -m http.server 8000`.

## Host on GitHub Pages
Settings > Pages > Deploy from branch > `main` / root.

## Roadmap (ideas for agents)
See `AGENTS.md`.
