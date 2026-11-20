# Student Grade Calculator

A simple web app that calculates a student's weighted course grade from quizzes, assignments and exams. Built with plain HTML, CSS and JavaScript. No installation or libraries needed.

## Features

- Add any number of assessments with a score, maximum marks and weight (%)
- Weighted percentage, letter grade (A to F with +/-) and 4.0 GPA
- Leave the score empty for upcoming work to see what you still need
- Target grade planner: shows the average you need on the remaining work, or tells you if the target is out of reach
- Warns when weights don't add up to 100%
- Progress bar with grade boundaries (60, 70, 80, 90)
- Saves your data in the browser automatically
- Works on phone and desktop, with light and dark mode

## How to run

1. Download or clone this repository
2. Open `index.html` in any browser

## How the grade is calculated

```
weighted % = sum(score / max x weight) / sum(weights of graded work) x 100
```

Only graded work (score filled in) counts toward the current grade. Needed average on remaining work:

```
needed % = (target x total weight / 100 - points earned) / remaining weight x 100
```

## Grade scale

| Percentage | Grade | GPA |
|-----------|-------|-----|
| 93+ | A | 4.0 |
| 90-92 | A- | 3.7 |
| 87-89 | B+ | 3.3 |
| 83-86 | B | 3.0 |
| 80-82 | B- | 2.7 |
| 77-79 | C+ | 2.3 |
| 73-76 | C | 2.0 |
| 70-72 | C- | 1.7 |
| 67-69 | D+ | 1.3 |
| 63-66 | D | 1.0 |
| 60-62 | D- | 0.7 |
| below 60 | F | 0.0 |

## Project structure

```
student-grade-calculator/
├── index.html   # app (HTML, CSS and JS in one file)
└── README.md
```

## Live demo

Enable GitHub Pages (Settings > Pages > Deploy from branch > `main` / root) and your app will be live at
`https://<your-username>.github.io/student-grade-calculator/`
