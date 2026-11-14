# Engineer Practical Trainer: handoff

Last updated 2026-11-14.

## What it is

A phone-first web page for memorizing the Engineer Practical Exam checklists (2026 Engineer Bibliography, pages 65-81). One file, `index.html`, plus `hero.jpg`. No build step, no accounts, no server; progress is saved in each phone's browser.

- Live: https://kwinter247.github.io/engineer-practical-trainer/
- Hosting: GitHub Pages from `main`. A push goes live in one to two minutes.

## What works

- Home screen: photo hero with title and "BY CODE3TEK", rank and XP, three daily missions, Study path button, practice tiles, exam readiness, light/dark toggle.
- Practice styles: Read and learn, What comes next?, Put in order, From memory (typed), Say it out loud (speech), Numbers round.
- Study path: the five sections in order with a Continue card.
- Content: 5 sections, 46 parts, 450 steps, 30 number questions.

## Not verified

- The step text was typed from the PDF and has not been proofread against the packet.
- Say it out loud was tested only with simulated speech, never with a real microphone. It needs Chrome on Android or Safari on iPhone.
- Whether the page now opens at the top on a phone, and whether the grey flash on load is gone, were not confirmed.
- The light/dark choice being remembered between visits was not confirmed.

## Known limits

- Speech matching is loose on purpose; in a simulated full run about 10 of 448 steps were marked a line early, none missed. Spoken fractions (4/32) do not match.
- The Pumping section has tasks only; the rationale column is not included.
- "Inside Cab" is split into three parts and the air brake test into two. "Wheel chalks" was corrected to "wheel chocks".

## Ideas not started

Exam simulation, proctor mode, a pumping "why" round, written-exam practice questions, spaced review of weak steps, a crew leaderboard, and importing any document.

## Working on it

- Open `index.html` directly, or serve the folder (`python -m http.server`) so `hero.jpg` loads.
- Content lives in the `DATA` and `NUMS` arrays at the top of the script; a leading `>` marks one level of indent.
- Ranks are in `RANKS`, missions in `MISSIONS`, colours in the `:root` blocks.
