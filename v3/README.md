# Focus Timer v3 (End of Cycle 1)

The third version of my Focus Timer. It builds on v2 (Week 4) and changes only the things that came up when two students tested v2.

**Live app:** https://battiribat.github.io/focus_timer/v3/
**v2 (Week 4):** https://battiribat.github.io/focus_timer/v2/
**v1 (Week 1):** https://battiribat.github.io/focus_timer/

## Design goal
I want students who study at home to finish what they planned for a session, without losing focus or having their flow cut off.

## Prototype testing
Two students from my Week 3 interviews used v2 in a real study session and answered four short questions after.

- T1: 2nd-year Economics student, at home, on her phone, before a midterm
- T2: 1st-year Management student, in the library, on his laptop (also opened it on his phone)

## What changed in v3 (and why)
| Change | Why (test finding) |
|---|---|
| The plan screen says to pick something you can finish in this session, and has quick-start buttons: "Solve _ questions", "Read pages _", "Summarize _". The example in the task field is also more concrete. | T1 did not know what to write as a task and wrote only the course name. |
| When time is up, "Keep going" now has two options: +10 min and +25 min. | T2's task took longer than he expected. |
| The break screen has a "Still working? Skip the break" button that goes straight back to focus. | T2 kept working during the break, but the app thought he was on a break. |

## What stayed the same
- Soft stop when time is up (T1 could still choose a break herself)
- Summary with tasks done and "Did you understand it?" (both testers said it matched their session)
- The overall flow (T2 made no wrong clicks)
- The phone check. Neither tester talked about it, so I keep it and test it again later.

## Tech
Plain HTML, CSS and JavaScript in one `index.html` file. No build step, no libraries.
The plan, the running timer and today's stats are saved in the browser (localStorage).
Hosted with GitHub Pages. Works on phone and desktop, supports dark mode.
