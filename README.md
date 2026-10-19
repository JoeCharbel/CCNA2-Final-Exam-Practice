# CCNA 2 Practice Quiz (SRWE)

A lightweight, browser-based practice quiz for **CCNA 2: Switching, Routing, and Wireless Essentials**. No installs, no backend, just open it and start practicing.

## Features

- 60 randomly selected questions per attempt, drawn from a pool of 160+
- Randomized question order and answer order on every retake
- Single-answer and multi-select questions
- Live timer, progress bar, and running score
- Results screen with score ring, time taken, and a review of every wrong answer with the correct answer and explanation
- Responsive dark UI

## How to run

No download or setup needed. Just use the live version:

1. 1. Open the [live demo](https://joecharbel.github.io/CCNA2-Final-Exam-Practice/).
2. Click **Start Quiz**.
3. Answer the 60 questions (multi-select questions are marked).
4. Review your score and any wrong answers with explanations at the end.
5. Click **Retake** for a new random set of questions.

## Run locally (optional)

You don't need to do this, since the live version above works in any browser. If you'd like an offline copy, clone the repo and open `index.html`. No build step or server is required.

## Adding or editing questions

Each question in `ccna2_questions_base.js` follows this format:

```js
{
  "question": "Which protocol adds security to remote connections?",
  "options": ["FTP", "HTTP", "SSH", "POP"],
  "correct": ["SSH"],
  "explanation": "SSH encrypts remote management sessions.",
  "multi": false
}
```

- `correct` must contain the exact text of the correct option(s).
- Set `multi` to `true` when more than one answer is correct.
- To change the number of questions per quiz, edit `QUESTIONS_PER_QUIZ` in `index.html`.

## Known limitations

- Some questions say "Refer to the exhibit" but the exhibit images are not included.

## Disclaimer

This is an unofficial study aid and is not affiliated with or endorsed by Cisco or Cisco Networking Academy.
