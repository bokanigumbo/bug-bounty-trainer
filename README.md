# bug-bounty-trainer🐛

a gamified, ai-powered bug hunting app built to help developers sharpen their debugging skills across multiple languages. spot the bug, explain the fix, earn xp and climb the leaderboard.

built with vanilla html, css, and javascript. no frameworks, no build tools and just one file you can open in a browser.

---

## what it does

the app generates real, deliberately broken code snippets using ai and challenges you to find and explain the bug. you're scored on accuracy, earn xp, and unlock badges as you improve.

- **multi-language support** — snippets in python, javascript, java, and c++
- **ai evaluation** — your answer is assessed by an llm that gives structured feedback and a score
- **two modes** — find the bug yourself, or switch to explain mode where the bug is described and you write the fix
- **difficulty scaling** — starts easy, introduces medium and hard snippets as you improve
- **category drill-down** — click any bug type in the categories tab to focus your practice on weak areas
- **difficulty voting** — rate how hard each snippet felt, aggregated across sessions
- **xp and levelling** — earn xp for correct and partial answers, level up from level 1 to level 6
- **streak tracking** — consecutive correct answers build your streak
- **badge system** — seven badges to unlock including `polyglot`, `hard_mode`, and `explainer`
- **activity heatmap** — github-style grid showing your bug-hunting activity over the last 6 months
- **weak spots tracker** — bar chart of your accuracy per bug type, sorted worst to best
- **leaderboard** — post your score and compete with others
- **share card** — copy your stats as text to share anywhere
- **dark mode** — respects your system preference automatically
- **persistent state** — xp, badges, activity, and stats are saved to localstorage between sessions

---

## bug types covered

| bug type | description |
|---|---|
| off-by-one error | loop or index is one step too far or short |
| null reference | accessing a variable or property that doesn't exist |
| logic error | code runs but produces the wrong result |
| type mismatch | wrong data type used in an operation |
| infinite loop | loop condition never becomes false |
| memory leak | resources allocated but never released |
| incorrect operator | wrong comparison or arithmetic operator used |
| missing edge case | code breaks on empty input, zero, or boundary values |
| scope error | variable used outside the block it was declared in |
| race condition | output depends on unpredictable timing between operations |

---

## tech stack

| layer | technology |
|---|---|
| frontend | vanilla html, css, javascript |
| ai | groq api — llama 3.3 70b |
| fonts | jetbrains mono (google fonts) |
| icons | tabler icons |
| storage | localstorage |
| hosting | github pages |

no npm, no webpack, no react. just one `.html` file.

---

## running it locally

1. clone or download this repo
2. get a free api key from [console.groq.com](https://console.groq.com)
3. open `bug_bounty_trainer.html` in a text editor and replace `YOUR_API_KEY_HERE` with your key
4. open the file in a browser

that's it. no server needed.

---

## project structure
bug-bounty-trainer/

  ├── bug_bounty_trainer.html   # the whole app — html, css, and js in one file

  └── README.md

  ---

## what i learned building this

- how to design a prompt that reliably returns structured json from an llm
- how to evaluate free-text answers programmatically using ai
- building a gamification system from scratch (xp, levels, streaks, badges)
- css custom properties for clean dark mode support
- persisting complex state (sets, nested objects) to localstorage
- how to make a single html file feel like a full product

---

## future ideas

- timed mode with score multipliers for speed
- session history log with searchable past attempts
- shareable profile url with encoded stats
- syntax highlighting on code snippets
- github readme export of your stats

---

## author

bokani — cs student at the university of liverpool

