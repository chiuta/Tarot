# Tarot — interactive course

**English** · [Română](README.ro.md) · [Français](README.fr.md) · [Italiano](README.it.md) · [Español](README.es.md) · [Português](README.pt.md) · [Deutsch](README.de.md) · [Magyar](README.hu.md)

**Version:** 1.1.0 · **Last updated:** 2026-10-14

A course in Romanian on the history, structure and practice of tarot, in a single HTML file, with no account and no server.

**Live app:** https://chiuta.github.io/Tarot/

![Screenshot](screenshot.png)

## What it is

A small interactive course on tarot as a cultural and symbolic tradition: history, the structure of the 78-card deck, four course levels with exercises, a comparison of traditions (Marseille, Rider-Waite-Smith, Thoth), a glossary, a journal and a self-assessment. Tarot is treated as a tool for reflection and entertainment, not as a scientific method.

## Features

Sections (left-hand menu, ☰ on mobile): Introduction, History, Structure of the deck, the four levels (Foundations, the Major Arcana with the Fool's Journey diagram, the Minor Arcana, Professional reading), Practical applications, Traditions and decks, Glossary, Journal, Self-assessment.

Verified in the code and in the browser:
- Random draw of 1 or 3 cards from a virtual 78-card deck (Fisher–Yates shuffle with `crypto.getRandomValues`, no repetitions); only the card names are shown; the result can be added to the journal.
- Choice of deck for the draw (full 78 / Major Arcana only, 22 / Minor Arcana only, 56); each drawn card also shows its structural membership ("Major Arcana" / "Minor Arcana"), without interpretations.
- Search within the course, diacritics-insensitive; each result shows a text excerpt with the term highlighted, and on selection the page scrolls to that spot and marks it.
- Direct link to a section (`#istoric`, `#quiz`, etc.); the browser's Back/Forward buttons work.
- Journal downloadable as `.txt` and "Upload (.txt)" (adds the text of a chosen file, up to 1 MB, to the current journal; nothing is saved in the browser); 10-question quiz with shuffled answer order.
- Printing (current section only), sharing/copying the link, full screen, keeping the screen awake (where the browser supports them).

## User guide

1. Choose a section from the menu (on mobile, tap ☰).
2. Read the levels in order and try the practical exercises.
3. In "Practical applications" press "Draw one card" or "Draw 3 cards"; the interpretation is up to you, with your own deck.
4. Take notes in the "Journal"; press "Download (.txt)" before closing the page — the journal is not saved.
5. In "Self-assessment" answer the 10 questions; "Retake the test" shuffles the answers again.

## Privacy and network

- Storage: it does not use `localStorage`, `sessionStorage`, IndexedDB or cookies. The journal exists only on the page; on closing/reloading the browser warns you if you have unsaved text.
- Network: it makes no external requests (no fonts, scripts, images or analytics). The page has a CSP policy (`default-src 'none'`) that blocks connections. There are no external links.
- Permissions: it asks for nothing on load. When you press buttons, the following may be used: full screen, wake lock (screen kept awake), clipboard (link copying) and vibration on mobile for quiz answers.

## Limits and warnings

- Tarot is a cultural tradition and a tool for reflection/entertainment. There is no scientific evidence that it can predict the future, diagnose or heal.
- The content is educational and does not replace the advice of a doctor, psychologist, lawyer or financial adviser. Do not give up a treatment and do not make important decisions on the basis of a draw.
- Historical claims are presented briefly; the lines about certifications and courses in Romania are marked as unverified.
- It does not include card images; the draw shows names only.

## History / Changelog

- 1.1.0 — 2026-10-14: Backup and data labelling (fff-kit).

- 1.0.0 — 2026-10-12: the version and the date of the last update are shown in the app
- Search now shows the excerpt in which the term appears (previously, queries such as "The Tower" showed only the section title) and highlights the match in the text on selection.
- Added: choice of deck for the draw, the Major/Minor Arcana label, "Upload (.txt)" in the journal; CSP: `script-src` by SHA-256 hash, no `'unsafe-inline'`; the card titles in "Structure of the deck" and "Practical applications" are now h3 (correct heading order in these two sections; axe-core: 0 violations on all 12 sections, 1280 px).
- The page now has a level-1 heading in the main area, visible to screen readers and on mobile (the side menu is hidden there); the visible appearance did not change. axe-core: 0 violations at 1280 and 360 px.
- The content remains without card images and without per-card interpretations (a content choice by the author, unchanged).

## Running locally / offline

Download `index.html` and open it in the browser; it works without internet.

## License

MIT — see the LICENSE file.

## Author

Alexio — Alexandru-Ionuț Chiuță, contact: alexio@trom.tf

## Summary

A single-file, offline course in Romanian on tarot as a cultural and symbolic tradition: history, the 78-card structure, four course levels, deck comparison, glossary, journal and a 10-question quiz, plus a random draw tool (Fisher–Yates with `crypto.getRandomValues`). No storage, no external requests, no telemetry. Tarot is presented as tradition and entertainment, with no scientific evidence of predictive power; it is not a substitute for medical, legal or financial advice. License: MIT (see the LICENSE file).
