# Undergrad E-Portfolio Tutorial

A free, ready-to-use portfolio template for students. No coding experience needed. No installs. Just edit the files and put it live on the internet in minutes.

**Scan the QR code below to open this project on GitHub, then fork it to get your own copy.**

![QR code to this GitHub repo](qr-code.png)

---

## What is in this project?

| File | What it does |
|------|-------------|
| `index.html` | Your home page — the first thing people see |
| `projects.html` | A page to show your projects |
| `skills.html` | A page to list your skills |
| `resume.html` | A page with your education and work history |
| `contact.html` | A page with your email and social links |
| `css/style.css` | Controls the colours and layout on every page |
| `images/` | Put your photos and screenshots here |
| `resume.pdf` | Upload your CV here as a PDF |
| `templates/` | 6 pre-made designs — pick one if you want a different look |
| `AI_PROMPTS.md` | Prompts to help you edit with ChatGPT or Claude |
| `HOSTING_GUIDE.md` | Step-by-step instructions to get your site live |

---

## How to get started

**Step 1 — Create a free GitHub account**
Go to [github.com](https://github.com), click **Sign up**, and create an account. Your username will appear in your website link, so pick something professional (e.g. `alex-johnson`).

**Step 2 — Get your own copy of this project**
Click the **Fork** button at the top right of this page. This copies the whole project into your own GitHub account so you can edit it freely.

**Step 3 — Turn it into a live website**
In your copy, go to **Settings → Pages → Source → main branch → Save**. GitHub will publish your files as a real website. It takes about 60 seconds.

**Step 4 — Find your live link**
After saving, refresh the Settings → Pages screen. Your link will appear — it looks like:
`https://your-username.github.io/undergrad-eportfolio-tutorial/`

**Step 5 — Edit the files to make it yours**
Click on any file (start with `index.html`), click the pencil icon to edit, replace the placeholder text, and click **Commit changes**. Your live site updates within a minute.

For photos, resume upload, and everything else, read [`HOSTING_GUIDE.md`](HOSTING_GUIDE.md) — it explains every step from scratch.

---

## The 6 themes

There are 6 pre-made designs for different fields. Each one is a **complete single-page portfolio** — everything (projects, skills, experience, contact) is on one page, and the menu scrolls you to each section.

Open `templates/index.html` to preview all 6 side by side before picking one.

| Template file | Best for |
|---------------|----------|
| `template-cs.html` | Computer Science / Software Engineering |
| `template-design.html` | Design / UX / Creative Arts |
| `template-data.html` | Data Science / Machine Learning |
| `template-bio.html` | Biology / Life Sciences / Pre-Med |
| `template-business.html` | Business / Finance / Consulting |
| `template-arch.html` | Architecture / Civil / Urban Design |

**To use a template:**
1. Open the template file on GitHub and click the pencil icon to edit
2. Press Ctrl+A (or Cmd+A on Mac) to select all, then copy
3. Open `index.html`, select all, paste, and commit

That's it — the template replaces `index.html` and contains everything. The other page files (`projects.html`, `skills.html`, etc.) are no longer needed when using a template.

For full instructions see [Part 8 of HOSTING_GUIDE.md](HOSTING_GUIDE.md).

---

## Change the colour scheme

Open `css/style.css` and change these 4 lines at the top. Every button, link, and highlight on every page will update.

```css
:root {
  --accent:      #2563eb;   /* main colour */
  --accent-dark: #1d4ed8;   /* hover colour */
  --bg:          #f8fafc;   /* page background */
  --surface:     #ffffff;   /* card background */
}
```

---

## Checklist — things to update after you fork

- [ ] Replace `Your Name` in all 5 HTML files
- [ ] Add your photo — upload `profile.jpg` into the `images/` folder
- [ ] Add your real projects in `projects.html`
- [ ] Fix the skill percentages in `skills.html`
- [ ] Add your real education and work history in `resume.html`
- [ ] Update your email, GitHub, and LinkedIn links in `contact.html`
- [ ] Upload your CV as `resume.pdf`
- [ ] Pick a colour — change `--accent` in `css/style.css`

---

## Why no JavaScript?

Everything — the mobile menu, progress bar animations, hover effects — works with CSS only. This means no installs, no setup, and no broken dependencies. If you want to add JavaScript later, `AI_PROMPTS.md` has prompts to help you do that.
