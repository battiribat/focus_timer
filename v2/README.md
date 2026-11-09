# Focus Timer v2 (Week 4 redesign)

The redesigned version of my Week 1 Focus Timer, based on my Week 3 research (context mapping and 3 short interviews with students) and my Week 4 lo-fi prototype.

**Live app:** https://battiribat.github.io/focus_timer/v2/
**Week 1 version:** https://battiribat.github.io/focus_timer/

## Design goal
I want students who study at home to finish what they planned for a session, without losing focus or having their flow cut off.

## What changed (and why)
| Change | Why (finding) |
|---|---|
| Every session starts with a plan of 1–3 small tasks | Students judge a session by tasks done or topics understood, not hours. Small tasks help focus. |
| "Phone on silent and out of reach" check before starting | The phone is the biggest distraction, even when it is just nearby. |
| The current task is always shown on the timer screen | After a distraction it is hard to remember where you were. |
| No hard stop when time is up: soft sound + "Keep going +10 min" or "Take a break" | Fixed Pomodoro alarms interrupt students when they are deep in a problem. |
| Break screen shows the task you come back to and counts time **over** the break | Planned 10-minute breaks often turn into 30 minutes. |
| Summary shows tasks done, asks "Did you understand it?", and moves unfinished tasks to the next plan | "Enough" = tasks finished / topic understood. Fast restart because students forget to open the app. |

## Screens
1. Plan session → 2. Focus → 3. Time's up (soft) → 4. Break → 5. Session summary

## Tech
Plain HTML, CSS and JavaScript in one `index.html` file. No build step, no libraries.
The plan, the running timer and today's stats are saved in the browser (localStorage), so a page refresh does not lose the session.
Hosted with GitHub Pages. Works on phone and desktop, supports dark mode.
