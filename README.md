# Undergrad E-Portfolio Tutorial

A complete, zero-dependency HTML/CSS portfolio template for undergrad students — designed for a 45-minute workshop talk.

**Live site → scan the QR code or visit:**
`https://yash-sukhdeve.github.io/undergrad-eportfolio-tutorial/`

![QR code to live site](qr-code.png)

---

## What's Included

| File | Purpose |
|------|---------|
| `index.html` | Home / About — hero, bio, quick stats |
| `projects.html` | Project cards with tech badges and GitHub links |
| `skills.html` | CSS-only progress bars, soft skill badges |
| `resume.html` | CSS-only timeline — education, experience, achievements |
| `contact.html` | Contact form (Formspree-ready) + social links |
| `css/style.css` | Single shared stylesheet — one variable change rethemes everything |
| `AI_PROMPTS.md` | Ready-to-use AI prompts for building and customising your portfolio |
| `generate_qr.py` | Regenerates `qr-code.png` if you change the URL |

---

## AI Prompts

**Not sure how to write a section? Just ask an AI.**

[`AI_PROMPTS.md`](AI_PROMPTS.md) has 30+ copy-paste prompts for ChatGPT, Claude, Gemini, or any AI assistant — covering everything from generating your bio to adding dark mode, animations, and JavaScript features.

Categories:
- Getting started & personalising the template
- Writing hero bio, project descriptions, resume bullet points
- Adding new sections (blog, certifications, open source)
- Changing colours, fonts, and themes
- Dark mode, animations, hover effects
- Debugging layout and contrast issues
- Going further with vanilla JavaScript

---

## Quick Start (for students)

1. **Fork** this repo on GitHub (button top-right).
2. Go to **Settings → Pages → Source → main branch / root** and save.
3. Your live URL will be `https://<your-username>.github.io/undergrad-eportfolio-tutorial/` within ~60 seconds.
4. Edit the files — start with `index.html` and replace all placeholder text.

---

## Retheme in One Line

Open `css/style.css` and change the four variables at the top:

```css
:root {
  --accent:      #2563eb;   /* ← change this to your favourite colour */
  --accent-dark: #1d4ed8;
  --bg:          #f8fafc;
  --surface:     #ffffff;
}
```

That's it — every button, link, progress bar and highlight updates automatically.

---

## Talk Outline

| # | Topic |
|---|-------|
| 1 | Why an e-portfolio? Jobs, internships, grad school |
| 2 | What pages to include and what content goes where |
| 3 | HTML/CSS quick refresher — structure vs style |
| 4 | Live walkthrough of this template |
| 5 | GitHub Pages setup — fork → Settings → live URL |
| 6 | Customisation tips — colours, fonts, projects |

---

## Customisation Checklist

- [ ] Replace `Your Name` everywhere
- [ ] Swap the placeholder photo in `index.html`
- [ ] Update the 3 project cards in `projects.html` with your real projects
- [ ] Adjust skill percentages in `skills.html`
- [ ] Fill in your real education / experience in `resume.html`
- [ ] Add your GitHub, LinkedIn, email in `contact.html`
- [ ] Create a free [Formspree](https://formspree.io) form and paste the ID into `contact.html`
- [ ] Upload a real PDF resume and link it in `resume.html`
- [ ] Change `--accent` in `css/style.css` to your preferred colour

---

## Design Decisions (for the talk)

- **No JavaScript** — every interaction (mobile nav, progress bars) uses CSS only. Nothing to install, nothing to bundle.
- **No external libraries** — loads instantly on any connection.
- **CSS Grid `auto-fit / minmax`** — the grid reflows automatically; no media queries per card needed.
- **CSS variables** — students see how a design token system works at the simplest possible scale.
- **Formspree** — a free tier that lets you collect contact form submissions without any backend code.

---

## Regenerating the QR Code

If you fork and rename the repo:

```bash
pip install qrcode[pil]
# edit the URL inside generate_qr.py first
python generate_qr.py
git add qr-code.png && git commit -m "update QR code"
```
