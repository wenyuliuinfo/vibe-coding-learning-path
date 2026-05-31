# AGENTS.md

## Project overview
Personal homepage for Eva Liu — a solution architect exploring AI Agents. Single-page prototype for collaborators, colleagues, and interviewers.

## Tech stack
- Single-file HTML + CSS + vanilla JS (no frameworks, no build step)
- No external dependencies or CDN imports
- Preview: `python3 -m http.server 8080` → `http://localhost:8080`

## Design constraints
- Professional, minimal, tech-forward
- Color palette: dark blue (#080c14 background) and black, with blue accents (#3b82f6, #60a5fa)
- Mobile-friendly (responsive grid, clamp-based sizing, breakpoint at 600px)
- Subtle dynamic effects only (particles, avatar ring spin, hover lifts, message fades)

## File structure
- `index.html` — the entire page (styles inline in `<style>`, scripts inline in `<script>`)
- `AGENTS.md` — this file

## Key sections in index.html
1. **Hero** — animated avatar ring, gradient name, one-line tagline
2. **About Me cards** — 3 cards: Current Focus, Interests, Work Style (CSS grid, responsive)
3. **Digital Avatar Chat** — chat UI with keyword-based Q&A bot, suggestion chips

## Chat bot behavior
- Keyword matching from a `knowledge` array in the inline script
- Scored by number of matched keywords; fallback reply if no matches
- Simulated typing delay (600–1000ms) before bot responds
- 3 suggestion chips map to the 3 most-expected questions:
  1. "What are you working on recently?"
  2. "What is your biggest strength?"
  3. "What AI Agent projects have you done?"

## Owner identity
- Name: Eva Liu
- Profession: Solution architect
- Focus: AI Agent projects, industrial AI solutions, enterprise AI Agent implementation
- Interests: AI news, traveling, reading
- Trait: Cross-discipline collaboration for AI implementation

## Conventions
- Keep the single-file approach unless explicitly asked to split
- No external fonts or icon libraries — use system fonts and emoji
- Dark theme only; do not add light mode
- Changes should stay consistent with the existing color palette and minimal aesthetic
