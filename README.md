# Calorie Tracker

A single-file web app for weight loss. No server, no sign-up, no dependencies. Your data stays in your browser (localStorage).

## What it does
- Calculates your daily calorie target (Mifflin-St Jeor BMR x activity level, minus a deficit for your goal pace)
- Logs food (calories, protein, carbs, fat)
- Logs weight and draws a 7-day moving average
- Compares predicted loss (from your intake) to actual loss (from your scale)

## Run it
Open `index.html` in any browser.

## Publish it free with GitHub Pages
Repo > Settings > Pages > Source: "Deploy from a branch" > Branch: `main` / root > Save.

## Notes
- 1 kg of fat is treated as about 7,700 kcal.
- Minimum target: 1,500 kcal (male) / 1,200 kcal (female).
- Estimates only, not medical advice.
