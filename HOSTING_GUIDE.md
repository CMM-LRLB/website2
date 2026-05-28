# How to Put Your Portfolio Live on the Internet

By the end of this guide, you will have a real website with a link you can share with anyone — for free.

Your link will look like this: `https://your-username.github.io/undergrad-eportfolio-tutorial/`

You do not need to install anything. You only need a browser.

---

## Part 1 — What Are All These Files?

When you open the project folder, here is what everything is:

```
undergrad-eportfolio-tutorial/
│
├── index.html          ← Your HOME PAGE. This is the first page people see.
├── projects.html       ← Your projects page
├── skills.html         ← Your skills page
├── resume.html         ← Your resume / work history page
├── contact.html        ← Your contact page
│
├── css/
│   └── style.css       ← Controls ALL the colours and layout across every page
│
├── images/             ← Put your photos and screenshots here
│   └── profile.jpg     ← Your profile photo — name it exactly this
│
├── resume.pdf          ← Your CV as a PDF — name it exactly this
│
├── templates/          ← 6 pre-made designs — pick one if you want a different look
│
├── README.md           ← Info shown on your GitHub page
├── AI_PROMPTS.md       ← Prompts to help you edit with ChatGPT or Claude
└── HOSTING_GUIDE.md    ← You are reading this
```

**Important:** File names matter. If your photo is called `Profile.jpg` instead of `profile.jpg`, it will not show up. Always use lowercase letters and no spaces.

---

## Part 2 — Create a GitHub Account

GitHub is a free website where you store and publish your code. Think of it like Google Drive, but for websites.

1. Go to **github.com**
2. Click **Sign up**
3. Enter your email, choose a password, and pick a username

**Choosing your username:** This will appear in your website link. Use your real name or initials — something you would not be embarrassed to show a teacher or employer. Example: `alex-johnson` or `ajohnson2026`.

Once you are in, leave that tab open.

---

## Part 3 — Get Your Own Copy of This Project

You need to make your own copy so you can edit it. This is called "forking."

1. Make sure you are logged into GitHub
2. Go to the project page: `https://github.com/AVHBAC/undergrad-eportfolio-tutorial`
3. Click the **Fork** button in the top-right corner
4. Leave the name as it is and click **Create fork**

You now have your own copy at `https://github.com/YOUR-USERNAME/undergrad-eportfolio-tutorial`

---

## Part 4 — Turn Your Files into a Live Website

This step tells GitHub to publish your files as a website.

1. Go to your forked copy on GitHub (the one with your username)
2. Click the **Settings** tab at the top
3. In the left menu, click **Pages**
4. Under **Source**, click the dropdown and select **Deploy from a branch**
5. Under **Branch**, select **main** and leave the folder as **/ (root)**
6. Click **Save**

Wait about 60 seconds, then refresh the page. You will see:

> Your site is live at `https://your-username.github.io/undergrad-eportfolio-tutorial/`

Click that link — your portfolio is now on the internet.

---

## Part 5 — Edit the Files to Make It Yours

Now you replace all the placeholder text with your real information.

### The easiest way — edit directly on GitHub

1. Go to your repo and click on `index.html`
2. Click the **pencil icon** (top right of the file) to edit
3. Change the text — replace anything that says "Your Name", "Your University", etc.
4. Scroll down, write a short note like *"Add my name"*, and click **Commit changes**
5. Your live site updates in about 30–60 seconds

Do this for each file: `index.html`, `projects.html`, `skills.html`, `resume.html`, `contact.html`.

### What to change in each file

**index.html** — your name, your university, your bio, your GitHub and LinkedIn links

**projects.html** — delete the 3 example projects and add your own (title, description, GitHub link)

**skills.html** — change the skill names and the percentage numbers to match your actual skills

**resume.html** — replace the education, experience, and achievements with yours

**contact.html** — update your email, GitHub link, and LinkedIn link

---

## Part 6 — Add Your Photo

Your photo will show on the home page. The HTML is already set up — you just need to upload the file.

1. Find a photo you want to use
2. **Rename the file to exactly:** `profile.jpg`
3. In your GitHub repo, click **Add file → Upload files**
4. A message says to upload into a folder — type `images/` before the file name so GitHub puts it in the right place. (If you just drag it to the root, move it into the `images` folder afterward.)
5. Click **Commit changes**

That is it. Refresh your live site and your photo will appear.

**If your photo is a PNG not a JPG:** rename it `profile.png` and in `index.html` change `profile.jpg` to `profile.png`.

---

## Part 7 — Add Your Resume PDF

1. Save your resume as a PDF (in Word: File → Save As → PDF; in Google Docs: File → Download → PDF)
2. **Rename the file to exactly:** `resume.pdf`
3. In your GitHub repo, click **Add file → Upload files**
4. Drag `resume.pdf` in and click **Commit changes**

The Download button on your resume page is already linked to `resume.pdf` — it will work automatically once the file is uploaded.

---

## Part 8 — Use a Different Design (Optional)

The default template has 5 separate pages (Home, Projects, Skills, Resume, Contact). The themed templates work differently — each one is a **single page** with everything on it, and the menu scrolls you to different sections instead of going to a new page.

There are 6 designs, one for each field. To see them all, open `templates/index.html` in your browser.

### Step 1 — Pick a template

| File | For |
|------|-----|
| `template-cs.html` | Computer Science / Software Engineering |
| `template-design.html` | Design / UX / Creative Arts |
| `template-data.html` | Data Science / Machine Learning |
| `template-bio.html` | Biology / Life Sciences / Pre-Med |
| `template-business.html` | Business / Finance / Consulting |
| `template-arch.html` | Architecture / Civil / Urban Design |

Click the file to open it and see what it looks like before you commit to it.

### Step 2 — Replace your index.html with the template

1. In your GitHub repo, click on the template file you want (e.g. `template-cs.html`)
2. Click the pencil icon to edit
3. Press **Ctrl+A** (Windows) or **Cmd+A** (Mac) to select everything, then copy
4. Go back to the root of your repo and open `index.html`
5. Click the pencil icon, press Ctrl+A / Cmd+A to select all, then paste
6. Click **Commit changes**

### Step 3 — Edit the placeholder text

The template has placeholder text just like the default — things like "Your Name", "Your University", "company name". Replace these with your real information.

### Note about the other HTML files

When using a themed template, you only need `index.html`. The files `projects.html`, `skills.html`, `resume.html`, and `contact.html` are no longer used — everything is inside `index.html`. You can ignore them or delete them.

---

## Part 9 — Change Your Website URL (Optional)

Right now your URL ends in `/undergrad-eportfolio-tutorial/`. You can shorten this.

In your repo, go to **Settings → General**, scroll to **Repository name**, and rename it to something like `portfolio`. Your URL becomes:

`https://your-username.github.io/portfolio/`

---

## Common Problems

**My changes are not showing on the live site.**

GitHub Pages takes 1–3 minutes to update. Wait and refresh. If it has been more than 5 minutes:
- Check Settings → Pages — is it still turned on?
- Did you click "Commit changes" after editing? Just editing without committing does not save anything.

**My photo is not showing.**

Check three things:
1. Is the file actually in the `images/` folder in your repo? Go look.
2. Is the file named exactly `profile.jpg`? Capital letters and typos will break it.
3. Did you commit the upload? Uploading without committing does not save.

**The Download Resume button does nothing.**

You have not uploaded `resume.pdf` yet. Follow Part 7.

**The page looks broken or has no colour.**

Check that `css/style.css` is still in your repo. Every HTML file needs this line near the top — make sure it has not been deleted:
```html
<link rel="stylesheet" href="css/style.css" />
```

**I accidentally deleted something.**

GitHub saves every version. Go to your repo, click the clock icon (**Commits**), find the last version that worked, and copy the old text back in.

---

## You Are Done

Once your site is live, the link never changes (unless you rename the repo). Every time you commit a change, the site updates automatically within a minute or two.

Put the link on your resume, your LinkedIn profile, and your email signature.
