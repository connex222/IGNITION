# CLAUDE.md - Ignition

Instructions for AI assistants working in this repository.

## What this is

A football warm-up app for grassroots coaches: ready-made 10-minute warm-ups, an exercise library with pictures, favourites, a coach mode and sound cues.

- Live: https://connex222.github.io/IGNITION/ (GitHub Pages, updates automatically from `main`)
- Audience: Grassroots football coaches on a touchline.

## Architecture

- **One self-contained file: `index.html`.** All CSS, JavaScript, fonts and artwork live inside it.
- State is saved in the browser's `localStorage`. Settings keys include `cbWarmCoachMode` and `cbWarmSoundCues`. Never rename an existing key without migrating the old data, or players lose their progress.

## Hard rules

- **Fully offline.** No network requests: no CDNs, no fonts or images from the internet, no analytics, no `fetch`.
- **No external dependencies.** Everything stays inside `index.html`.
- Readable in direct sunlight and in the dark (provide both light and dark themes with strong contrast).
- Works one-handed on a phone in portrait, and safe to interrupt at any moment without losing progress.
- Free to use. Do not add adverts, tracking or sign-ups.

## Project notes

- The file is large (about 9 MB) because the exercise pictures are embedded inside it. Compress any new picture before embedding it, and never link to images on the internet.
- Use correct UK grassroots football terms and age-appropriate content (FA guidance).

## Working with Shaun (the owner)

- Shaun is not a programmer. Explain every step in plain English, in order, and assume no prior knowledge.
- Always return the complete `index.html`, never partial snippets or "..." placeholders.
- Use UK English.
- Before saying a change is finished, check that the file still opens with no errors in the browser console.
- Never force-push, rewrite history or rename the repository.
