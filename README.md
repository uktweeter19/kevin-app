# Kevin - Fitness Tracker

Adult fat-loss focused fitness tracker. Single-file HTML app, no build step.

## Features

- **Home dashboard** with today's workout, calories, macros, hydration, and weekly set count
- **Weekly program** with gym, home, and family workout tracks - geared toward fat loss and definition for adults (no running; all cardio is incline walking)
- **Log workouts** by exercise with multi-set support
- **Personal Records** for lifts (squat, bench, OHP, row, goblet squat, pull-ups, push-ups, plank) and body metrics (body fat %, waist, chest, resting HR, 5K walk time, incline walk distance)
- **Body Fat Calculator** built in (YMCA method - margin of error +/- 3-4%)
- **Workout history** - last 30 days, grouped by date
- **Hydration tracker** with daily cup goal
- **Nutrition & macros** with calories, protein, carbs, fat, fiber, sugar, sodium - bodyweight-based cutting macros
- **Barcode scanner** - point camera at any UPC, auto-fills nutrition from Open Food Facts
- **Family food sync** - foods scanned or added by anyone (Kevin, Lincoln, Camille, Carter) sync via Firebase so nobody re-enters the same food twice
- **Fat-loss goals** that auto-update as PRs are logged
- **All workout data saves locally** in the browser via localStorage; food library syncs to the family Firebase

## How to Use

Visit `https://kevin.deatheragefamily.com` on any modern browser. Add to home screen for an app-like experience.

1. Enter height, weight, and target weight on the Home tab
2. Log any PRs you already have on the Records tab
3. Hit GYM, HOME, or FAMILY on the home screen to jump into today's workout
4. Tap LOG next to any exercise to record your sets
5. In the Fuel tab, tap SCAN BARCODE to scan packaged foods, or use the search/custom tabs

## Tech

Single HTML file. No build step. Dependencies loaded from CDN:

- Google Fonts (Barlow / Barlow Condensed)
- ZXing Browser (barcode scanning)
- Firebase Realtime Database via REST API (family food sync)

Works in any modern browser. Requires HTTPS for camera and Firebase access.
