# PawTrack — Animal Safety, Tracking & Rescue

PawTrack is a student prototype for a social-cause project. It demonstrates a community reporting interface for missing animals, injured animals, animal sightings, and road-risk/near-miss locations.

## Features in this prototype
- Create reports with animal type, location/landmark, date/time, description, optional contact, and optional photo.
- Browse, search, and filter reports.
- View dashboard counts by report type and status.
- Mark reports as resolved.
- Sample reports are included and labelled as samples.
- Data is saved in the current browser using `localStorage`.

## Run locally
1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. No build tools or API keys are required.

For a more consistent local development server, run:
```bash
python -m http.server 8000
```
Then open `http://localhost:8000`.

## Important limitations
This is a front-end demonstration only. Reports remain in the browser that created them; they are not shared with other users and are not delivered to rescue teams. The image matching and road-risk prediction features are represented as planned capabilities, not implemented AI models. Do not use this demo for emergencies. Contact local animal welfare/rescue services directly when an animal is in immediate danger.

## Suggested next steps
- Add a secure backend and database for shared reports.
- Add authentication, moderation, consent, privacy controls, and spam prevention.
- Integrate a mapping provider and geocoding with user permission.
- Validate road-risk scoring with reliable, reviewed incident and near-miss data.
- Train/evaluate image similarity on appropriately consented animal images before presenting it as AI.
- Build verified rescue-organization workflows and notifications.
- Add automated tests and accessibility checks.

## Project structure
- `index.html` — page structure and form
- `style.css` — responsive visual design
- `app.js` — report creation, filtering, status updates, and local persistence
- `docs/TECHNICAL_DESIGN.md` — architecture and data flow
- `data/sample-reports.json` — example reports for documentation/testing
- `LICENSE` — MIT License
