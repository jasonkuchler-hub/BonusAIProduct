# BonusAIProduct
# Study Session Tracker

A small, self-contained study timer. Set a study length and a break length,
start a session, and it logs what you worked on automatically when the timer
finishes. Your history (hours studied, current streak, a 7-day chart, and a
list of recent sessions) is saved locally in your browser.

## How to run it

No installation, no server, no dependencies.

1. Download `index.html`.
2. Double-click it (or open it from your browser with `File > Open`).

That's it — it runs entirely in the browser tab.

## How it works

- Set **Study (min)** and **Break (min)**, optionally type a **Subject**,
  and click **Start studying**.
- When the study timer reaches zero, the session is automatically logged
  (subject, duration, and timestamp) and you're offered a break.
- **Pause / Resume** works mid-session. **Stop** cancels the current session
  without logging it.
- Your data persists across browser refreshes using `localStorage` — it's
  stored only on your own machine, in that specific browser. Opening the
  file in a different browser (or a private/incognito window) will show an
  empty history, since `localStorage` doesn't sync across them.
- **Clear all data** permanently erases your logged sessions (with a
  confirmation prompt first).

## Notes

- Built as a single `index.html` file — all HTML, CSS, and JavaScript live
  in one place, so it's easy to drop into any repo or share as one file.
- No external libraries, fonts, or network requests — it works fully
  offline.
