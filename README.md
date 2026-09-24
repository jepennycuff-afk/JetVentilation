# HFJV Simulator — Monsoon III Jet Ventilation

An interactive training tool for **high-frequency jet ventilation (HFJV)** with the Monsoon III jet ventilator during interventional radiology (IR) procedures.

**Live site: https://jepennycuff-afk.github.io/JetVentilation/**

> ⚠️ **Training simulation only.** Always follow your institution's live protocol.

## Who it's for

Anesthesia residents, CRNAs, nurses and anesthesia techs who set up or run jet ventilation cases in IR.

## What's inside

| Tab | What you do there |
|---|---|
| **Overview** | The golden rule, HFJV in 30 seconds, a one-screen case timeline, and how patient orientation changes the room setup |
| **Setup** | A step-by-step checklist (5 phases). Ticks are saved on your device |
| **Simulator** | Run the jet, stabilize TcCO₂, take the initial scan (which locks settings), then practice events: rising CO₂, desaturation, and a PP/PIP alarm with a hidden cause to find |
| **Scenarios** | Short multiple-choice decision drills with explanations. Answers are shuffled every time |
| **Quick Reference** | Settings, CO₂ and oxygen flowcharts, alarm troubleshooting, contacts, documentation, end-of-case steps, glossary. Printable |

Tap any dotted-underlined abbreviation (DP, TOF, APL…) to see its definition.

You can link straight to a tab, e.g. `…/JetVentilation/#simulator` or `#reference`.

## Install it like an app

Open the live site on your phone, then:

- **iPhone (Safari):** tap Share → **Add to Home Screen**
- **Android (Chrome):** tap ⋮ → **Add to Home screen** (or **Install app**)

It gets the lung icon and opens full-screen without the browser bars.

## Editing the content

Everything lives in one file, `index.html`. The protocol content is kept in data blocks near the top of the `<script>` section, so each fact is written once:

- `SETTINGS` / `OTHER_SETTINGS`: default jet settings and ranges (used by the checklist, simulator and reference table)
- `SETUP`: the setup checklist phases and items
- `GLOSSARY`: abbreviations and definitions
- `ORIENT`: head-to-scanner vs feet-to-scanner notes
- `scenarios`: the quiz questions (`takeaway` is the one-line answer; `feedback` is the longer "Why?")

To preview locally, just open `index.html` in a browser. Changes pushed to `main` publish to the live site through GitHub Pages.

## Images

All images are in `assets/`:

| File | Used for |
|---|---|
| `how-it-works.jpg` | Conventional vs jet breathing (Overview) |
| `room-head-to-scanner.jpg`, `room-feet-to-scanner.jpg` | Patient orientation cards (Overview) |
| `ett-adapter.jpg` | Labeled ETT + swivel adapter illustration (Setup, step 2) |
| `ett-adapter-photo.jpg` | Real photo of the assembled tube (Setup, step 2) |
| `icon-*.png` | Scenario card icons |
| `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`, `favicon-32.png` | Home-screen app icon and browser tab icon |

The illustrations were generated with Google Gemini. Labels are added in the page rather than in the images, so they stay accurate.
