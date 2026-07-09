# SIM — Security Incident Mapping

A lightweight web platform that allows students, staff, and landlords to
quickly and anonymously report security incidents on and around campus.

Built for **SEN202 Weekly Dev — Weekend 1** (Dr. O. O. Ajayi).

## Live Demo
Open `webapp/index.html` in a browser, or enable GitHub Pages on this repo
(Settings → Pages → deploy from `/webapp` folder) to get a live link.

## Repository Structure
```
├── webapp/                     # Mini web interface (HTML/CSS/JS)
│   ├── index.html
│   ├── style.css
│   └── app.js
├── SIM_SRS.docx                 # Software Requirements Specification
├── SUPPORTING_ARTIFACTS.md      # Ishikawa content, Google Form structure, use-case description
└── README.md
```

## Problem
Insecurity linked to community/campus crime (theft, assault, and worse) is
under-reported due to the lack of a fast, low-friction, and anonymous
reporting channel. SIM addresses this gap.

## Features (MVP)
- Submit an incident report (type, location, date/time, description)
- Option to report anonymously or leave contact details
- View a live feed of reported incidents

## Tech Stack
Plain HTML, CSS, and JavaScript — no build step required. Data is stored
client-side (browser localStorage) for this prototype.

## Related Artifacts
- **Ishikawa Diagram**: causes analysis for campus/community crime — see https://github.com/KLASSICVKAY/SIM-security-incident-mapping/blob/main/Mind-14-34-55.png 
- **Use-Case Diagram**: see https://github.com/KLASSICVKAY/SIM-security-incident-mapping/blob/main/IMG-20260709-WA0124.jpg .
- **Google Form**: questionnaire structure for students, staff, and landlords — see https://docs.google.com/forms/d/1SiZQ0WdeOKh0Sx5nPao0jgpyOGFtrGeGmkg33fVQjOU/viewform
- **SRS Document**: https://github.com/KLASSICVKAY/SIM-security-incident-mapping/blob/main/SIM_SRS.docx
