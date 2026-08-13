# Bikroy Mobile Command

A single-page mobile dashboard for keeping an eye on the Bikroy ad-review team from a phone.

## What it does

This is the companion screen to the [Bikroy Ad Tracker](https://github.com/roni2026/bikroy-extension) browser extension. The extension does the actual review-queue automation on a desktop; this page is what a supervisor opens on their phone to check on it without needing the extension installed.

- Start/stop tracking and pick which agents are active, from a mobile-friendly bottom sheet
- Live queue counts shown as pills across the top of the screen
- Per-agent grid showing current status at a glance
- Activity log view for a history of what's happened
- Reads and writes the same Firebase Realtime Database as the extension, so both stay in sync instantly

## Tech stack

Plain HTML/CSS/JS — no build step. Tailwind is pulled in via CDN, icons via Font Awesome, and live data comes straight from Firebase's JS SDK.

## Using it

Open `agentdashboard_mobile.html` directly in a mobile browser, or host it as a static file. It needs the same Firebase project configuration as the browser extension to connect to — wire that in wherever the page initializes Firebase.
