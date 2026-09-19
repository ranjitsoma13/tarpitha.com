# Tarpitha

**Wisdom to live well** — a weekly collection of life lessons and timeless insights.

🌐 Live at [tarpitha.com](https://tarpitha.com)

---

## How it works

The site is a single HTML page (`index.html`) that reads all lessons from `lessons.json`. No code changes are needed to publish new content — just update the JSON file each week.

---

## Adding a new lesson every week

1. Open `lessons.json` in this repo
2. Click the **pencil icon** (Edit)
3. Add a new entry at the **top** of the array (before the first `{`):

```json
{
  "id": 2,
  "date": "2026-09-26",
  "theme": "Attention",
  "title": "Your lesson title here",
  "body": "First paragraph of your lesson.\n\nSecond paragraph. Add as many as you like, separated by \\n\\n."
},
```

4. Click **Commit changes**
5. tarpitha.com updates within 1–2 minutes ✅

### Rules to follow
- `id` — increment by 1 each week (1, 2, 3 …)
- `date` — use the format `YYYY-MM-DD`
- `theme` — pick one: Equanimity, Attention, Belonging, Impermanence, Character
- `body` — separate paragraphs with `\n\n`

---

## File structure

```
tarpitha.com/
├── index.html       # The website (do not edit unless redesigning)
├── lessons.json     # All lessons — edit this every week
├── CNAME            # Points the domain to GitHub Pages
└── README.md        # This file
```

---

## Themes

| Theme | Meaning |
|-------|---------|
| Equanimity | Remaining steady in pleasure and adversity alike |
| Attention | What we give focus to becomes our life |
| Belonging | Ties to people, place, and purpose |
| Impermanence | Accepting the transient nature of things |
| Character | Habits and values built slowly over a lifetime |

---

## Technical setup

- Hosted on **GitHub Pages** (free)
- Domain managed on **Squarespace** (tarpitha.com)
- No frameworks, no build step — pure HTML, CSS, and JavaScript
- Lessons stored in a plain JSON file — no database needed
