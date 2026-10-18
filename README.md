# PhishGuard

An interactive phishing-awareness training app built as Task 2 of the CodeAlpha Cyber Security Internship.

The staged course teaches users to recognise phishing emails and fake websites, understand social-engineering tactics, and apply safer habits with an interactive scored quiz.

---

## Live Demo

`https://244star.github.io/CodeAlpha-PhishGuard/`

*(To publish the demo, enable GitHub Pages in Settings > Pages and deploy from the `main` branch, root folder.)*

---

## What's Inside

| Section | What it covers |
|---------|----------------|
| **Spot the phish** | A mock phishing email. Click the suspicious parts to reveal the 5 red flags and why each matters. |
| **How attackers manipulate you** | Social engineering levers: urgency, authority, fear, reward, familiarity, plus smishing, vishing and QR-code phishing. |
| **Recognising fake websites** | Checking domains, spotting typosquatting, and why the padlock does not prove a site is safe. |
| **Real-world examples** | Twitter 2020 vishing attack, Google and Facebook invoice fraud, and the 2016 US campaign email hack. |
| **Best practices** | Practical habits: pause, verify, use MFA and a password manager, report, and what to do after clicking. |
| **Quiz** | 6 multiple-choice questions with instant feedback, explanations, and a final score with retry. |
| **Game-style progress** | Move through ordered stages, earn XP for spotting red flags and correct answers, and earn completion badges. |
| **Sound and motion** | Optional sound effects and lightweight transitions; reduced-motion preferences are respected. |

---

## Learning Objectives

After completing the module, a user should be able to:

1. Identify common warning signs in phishing emails.
2. Tell a genuine website address from a look-alike.
3. Recognise the psychological tactics used in social engineering.
4. Respond correctly to a suspicious message, or after falling for one.

---

## Running Locally

No installation or dependencies are required.

```bash
git clone https://github.com/244star/CodeAlpha-PhishGuard.git
cd CodeAlpha-PhishGuard
```

Then open `index.html` in any modern browser, or serve it locally:

```bash
python3 -m http.server 8000
# visit http://localhost:8000
```

---

## Project Structure

```
PhishGuard/
├── index.html    # the full module (HTML, CSS and JavaScript in one file)
└── README.md
```

---

## Technologies

- HTML5
- CSS3 (responsive layout, keyboard-visible focus styles)
- Vanilla JavaScript (staged navigation, XP, optional Web Audio feedback, interactive exercises and quiz; no libraries)

---

## Customising

- **Quiz questions:** edit the `questions` array in the script at the bottom of `index.html`. Each item has a question (`q`), options (`o`), the correct index (`a`) and an explanation (`w`).
- **Red flags:** update `flagInfo`, add a `data-f` attribute to the suspicious text and a matching `<li data-f="...">` in the flags list. Update the five-flag completion check if you change the total.

---

## Disclaimer

The email and website examples are fictional and created for training only. Real-world incidents are simplified summaries of publicly reported events.

---

## Author

Your Name
CodeAlpha Cyber Security Intern

## License

MIT
