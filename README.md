# Smart BP Monitor: HCI Redesign

A redesigned blood pressure monitor interface, built for an Human-Computer Interaction assignment. The original device was evaluated against **Nielsen's 10 usability heuristics**, and this prototype fixes the problems found, with a focus on **elderly users**.

**Live demo:** `https://YOUR-USERNAME.github.io/bp-monitor-hci/`

## What it does

A fully interactive, single-file prototype (HTML, CSS, JavaScript, no dependencies):

1. **Guided measurement:** three clear steps (sit, wrap cuff, stay still) with large text and tips
2. **Cuff placement check:** stops before measuring and shows exactly how to fix the problem
3. **Live progress:** animated progress ring while the cuff inflates and deflates
4. **Plain-language results:** Systolic, Diastolic and Pulse with a colour-coded scale (green, yellow, red) and advice such as "Please consult a doctor"
5. **Sound feedback:** unique sounds for each button, pump motor and air release while measuring, and different result jingles for normal, elevated and high readings
6. **Voice instruction bar:** on-screen guidance on every screen

Press **NEW READING** to cycle through four scenarios: Normal, Elevated, High Stage 1, High Stage 2.

## Heuristic evaluation, problems and fixes

| # | Heuristic | Problem in old device | Fix in redesign |
|---|-----------|----------------------|-----------------|
| 1 | Visibility of system status | No feedback during measurement | Progress ring, step dots, pump sounds |
| 2 | Match with real world | "120/80" is hard to understand | Plain labels (Normal / Elevated / High) and advice |
| 3 | User control and freedom | No easy cancel or redo | CANCEL, BACK and TRY AGAIN on every screen |
| 4 | Consistency and standards | Inconsistent symbols and colours | Standard green / yellow / red coding everywhere |
| 5 | Error prevention | Wrong cuff still gives a reading | Placement check before measuring |
| 6 | Recognition over recall | Users must remember how to wear the cuff | Step-by-step guidance on each screen |
| 7 | Flexibility and efficiency | Hard to access past data | Quick, simple flow with one primary action per screen |
| 8 | Minimalist design | Too many numbers and icons | Only Systolic, Diastolic, Pulse, large and clean |
| 9 | Error recovery | Unclear error messages | Plain explanation plus specific fix steps |
| 10 | Help and documentation | Relies on a paper manual | Voice and on-screen help, sound cues |

## Run locally

Open `index.html` in any modern browser. Sound starts after the first click (browser rule).

## Tech

Vanilla HTML, CSS and JavaScript. Sounds are generated with the Web Audio API, so there are no audio files.

## Author

Anirudra, Design student
