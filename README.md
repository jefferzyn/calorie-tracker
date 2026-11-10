# Calorie Tracker

A single-file web app for weight loss. Accounts and tracker data stay in the current browser using localStorage; there is no backend or password recovery.

## What it does
- Calculates your daily calorie target (Mifflin-St Jeor BMR x activity level, minus a deficit for your goal pace)
- Logs food (calories, protein, carbs, fat)
- Logs weight and draws a 7-day moving average
- Compares predicted loss (from your intake) to actual loss (from your scale)
- Creates a local account and keeps each user's tracker data separate
- Recommends recipe ideas from TheMealDB and estimates calories/macros by meal type
- Searches Open Food Facts by food or brand and looks up products by barcode
- Scales database nutrition to a chosen serving size before adding it to the diary

## Run it
Open `index.html` in any browser, or serve the folder locally with `python3 -m http.server 8000` and visit `http://localhost:8000`.

## Publish it free with GitHub Pages
Repo > Settings > Pages > Source: "Deploy from a branch" > Branch: `main` / root > Save.

## Notes
- 1 kg of fat is treated as about 7,700 kcal.
- Minimum target: 1,500 kcal (male) / 1,200 kcal (female).
- Estimates only, not medical advice.
- Recipe nutrition is estimated for planning; use the linked recipe and adjust portions for more accurate values.
- TheMealDB is an external service. The meal planner falls back to local suggestions if it is unavailable.
- Open Food Facts is an external service. Search and barcode errors leave quick add available as a fallback.
