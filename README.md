[README.md](https://github.com/user-attachments/files/33655515/README.md)
# CCNA 2 Practice Quiz (SRWE)

A lightweight, browser-based practice quiz for **CCNA 2: Switching, Routing, and Wireless Essentials**. No installs, no backend, just open it and start practicing.

**Live demo:** https://YOUR-USERNAME.github.io/REPO-NAME/

## Features

- 60 randomly selected questions per attempt, drawn from a pool of 160+
- Randomized question order and answer order on every retake
- Single-answer and multi-select questions
- Live timer, progress bar, and running score
- Results screen with score ring, time taken, and a review of every wrong answer with the correct answer and explanation
- Responsive dark UI

## Topics covered

VLANs and trunking (DTP, VTP), inter-VLAN routing, STP/RSTP/PVST+, EtherChannel (LACP/PAgP), DHCPv4 and DHCPv6, SLAAC, FHRP/HSRP, LAN security (port security, DHCP snooping, DAI), WLAN fundamentals and security, static routing and floating static routes, and routing troubleshooting.

## Project structure

| File | Purpose |
| --- | --- |
| `index.html` | UI, styling, and quiz logic |
| `ccna2_questions_base.js` | Question bank (`window.CCNA2_BASE_QUESTIONS`) |

## Run locally

Clone the repo and open `index.html` in any browser. No build step or server is required.

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
