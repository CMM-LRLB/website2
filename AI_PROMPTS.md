# AI Prompts for Building Your E-Portfolio

Copy any prompt below into **ChatGPT, Claude, Gemini, or any AI assistant**.
Replace the text inside `[ ]` with your own details before sending.

---

## Table of Contents

1. [Getting Started](#1-getting-started)
2. [Hero Section](#2-hero-section)
3. [Projects](#3-projects)
4. [Skills](#4-skills)
5. [Resume / Timeline](#5-resume--timeline)
6. [Contact Page](#6-contact-page)
7. [Design & Themes](#7-design--themes)
8. [Dark Mode](#8-dark-mode)
9. [Animations](#9-animations)
10. [New Sections](#10-new-sections)
11. [Debugging & Fixes](#11-debugging--fixes)
12. [Going Further (JavaScript)](#12-going-further-javascript)

---

## 1. Getting Started

### Generate a full portfolio from scratch

```
I am a [year, e.g. "third-year"] undergraduate student studying [your major]
at [your university]. I want to build a personal portfolio website using only
HTML and CSS (no JavaScript frameworks, no build tools).

My name is [Your Name]. My interests are [e.g. "machine learning, web development,
open source"]. I have done [number] projects and [number] internships.

Please generate:
1. index.html  — hero section with my name, a short bio, and a call-to-action button
2. css/style.css — a clean, modern stylesheet using CSS variables so I can retheme
   it by changing one line

Use a colour accent of [your favourite hex colour, e.g. #2563eb].
Make it mobile-responsive using CSS Grid. No JavaScript required.
```

---

### Personalise the template I already have

```
I have an HTML/CSS portfolio template. Here is my index.html:

[paste your index.html here]

Please update it with these details about me:
- Name: [Your Name]
- University: [University Name], [City]
- Degree: [e.g. B.Tech Computer Science]
- Graduation year: [year]
- Short bio (2–3 sentences): [write your bio here]
- Interests: [list them]
- Accent colour I want: [hex colour]

Keep the same HTML structure. Only change the content and the CSS variable --accent.
```

---

## 2. Hero Section

### Write a compelling bio paragraph

```
Write a 3-sentence "About Me" paragraph for a portfolio website.

About me:
- I study [your major] at [university]
- I am passionate about [topic 1] and [topic 2]
- I have worked on [a project or internship] where I [what you did]
- My career goal is to [goal]

Make it sound confident but not arrogant. Write in first person.
Avoid buzzwords like "passionate" and "leverage". Keep it under 60 words.
```

---

### Add a typing animation to the hero (CSS only)

```
I have this hero heading in my portfolio:

  <h1>Hi, I'm <span>Your Name</span></h1>

Add a CSS-only typewriter animation to the <span> so it types out my name
letter by letter on page load. Use @keyframes and the steps() timing function.
No JavaScript. Show me only the CSS to add and where to put it.
```

---

### Add a profile photo with a circular frame

```
In my portfolio's hero section I want to display a circular profile photo.
The photo file is called "photo.jpg" and is in the root of the project.

Add an <img> tag with:
- circular crop using border-radius
- a coloured ring border using CSS variable --accent
- a slight box-shadow for depth
- responsive sizing (shrinks gracefully on mobile)

Show me the HTML and CSS to add. My current --accent colour is [hex].
```

---

## 3. Projects

### Generate a project card

```
Add a project card to my portfolio's projects.html page.

Project details:
- Title: [Project Title]
- One-line description: [what it does]
- Tech stack: [e.g. Python, Flask, PostgreSQL, React]
- GitHub link: [URL]
- (optional) Live demo link: [URL or "none"]

The card should match the existing style: white background, border-radius,
box-shadow on hover, tech stack shown as pill badges. Show me just the HTML
block to paste inside the existing .grid div. No new CSS needed.
```

---

### Add a "Featured" badge to your best project

```
I have project cards in my portfolio. I want to mark one card as "Featured"
with a small coloured badge in the top-right corner of the card.

The card's container already has position: relative.
Use CSS only (no JavaScript). The badge should say "Featured" in white text
on a background of my --accent colour.

Show me the HTML to add inside the card and the CSS to add to my stylesheet.
```

---

### Add a live demo button alongside the GitHub button

```
My project cards currently have one button: "View on GitHub".
I want to add a second button: "Live Demo" that opens a new tab.

Demo URL: [your URL]

The "Live Demo" button should use the filled style (.btn) and the
GitHub button should use the outline style (.btn-outline), so they
look visually distinct side by side.

Show me the updated HTML for one card's button row.
```

---

## 4. Skills

### Add a new skill bar

```
I have CSS skill progress bars in my skills.html. Here is one example:

  <div class="skill-item">
    <label><span>Python</span><span>90%</span></label>
    <div class="skill-bar">
      <div class="skill-bar-fill" style="width:90%"></div>
    </div>
  </div>

Add the following new skills in the same format:
- [Skill 1]: [percentage]%
- [Skill 2]: [percentage]%
- [Skill 3]: [percentage]%

Return only the HTML blocks to paste.
```

---

### Replace progress bars with star ratings

```
I have CSS progress bar skill items in my portfolio. I want to replace
the bars with a 5-star rating display using CSS only (no JavaScript, no images).

Stars should be filled in with --accent colour up to the rating, and empty
(light grey) for the remainder.

For example: Python — 4.5 / 5 stars

Show me how to update one skill item's HTML and the CSS to add.
The approach must work without any icon library or font.
```

---

### Add a tools / technologies grid (logos)

```
Below my skill bars I want a "Tools I Use" section showing technology logos
in a responsive grid. I only have HTML and CSS (no JavaScript).

Technologies to include (use their text abbreviations as placeholders
since I'll swap in real SVG logos later):
[list your tools, e.g. VS Code, Git, Docker, AWS, Figma, Linux]

Create a grid that:
- Shows 4–5 items per row on desktop, 3 on tablet, 2 on mobile
- Each item is a small rounded card with the tool name centred
- Uses --accent colour on hover
- Uses CSS Grid auto-fit / minmax

Show me the HTML to add to skills.html and the CSS to add to style.css.
```

---

## 5. Resume / Timeline

### Generate a timeline entry

```
Add a new entry to my CSS-only resume timeline. Here is an existing entry
for reference:

  <div class="timeline-item">
    <div class="timeline-dot"></div>
    <h4>Software Engineering Intern</h4>
    <p class="meta">Company Name | May 2025 – Jul 2025</p>
    <p>Description here.</p>
  </div>

New entry details:
- Role / Degree: [title]
- Organisation: [company or university]
- Date range: [e.g. Jun 2024 – Aug 2024]
- 2-sentence description: [what you did and one concrete result/number]

Return only the HTML block.
```

---

### Write a bullet-point description for a work experience

```
Write 2–3 bullet points for a resume timeline entry describing this internship:

- Company: [company name]
- Role: [your role]
- Duration: [dates]
- What I worked on: [describe in plain language]
- One measurable result (if any): [e.g. "reduced load time by 30%"]

Format as short, action-verb-first sentences (past tense).
Each bullet point should be under 20 words.
Keep it factual and specific — avoid vague phrases like "contributed to" or "assisted with".
```

---

### Add a "Download CV" button that triggers a PDF download

```
I have a resume.html page. I want to add a "Download CV" button that downloads
a file called "resume.pdf" from the root of my project.

The button should:
- Use the .btn class (already in my stylesheet)
- Use the HTML download attribute so it triggers a download instead of opening in browser
- Say "Download PDF" with a small download icon (use a Unicode character, no icon library)

Show me only the HTML for the button.
```

---

## 6. Contact Page

### Activate the Formspree contact form

```
I have a contact form in contact.html. The form currently has:

  <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">

My Formspree form ID is: [your ID from formspree.io]

1. Update the action URL with my real ID.
2. Add a hidden redirect field so after submission the user is sent back to contact.html.
3. Add a honeypot field to reduce spam (Formspree supports _gotcha).

Show me the updated opening <form> tag and the hidden fields to add inside it.
No other changes needed.
```

---

### Add a "Thank you" message after form submission (CSS only)

```
My contact form submits to Formspree. After submission Formspree adds
?success=true to the URL. I want to show a "Thank you!" message using
only HTML and CSS — no JavaScript.

I can read URL parameters with the CSS :target selector trick, or use
a hidden element that becomes visible. Suggest the simplest CSS-only approach
and show me the HTML and CSS to add to contact.html.
```

---

## 7. Design & Themes

### Change the colour scheme

```
I have a CSS portfolio with these root variables:

  :root {
    --accent:      #2563eb;
    --accent-dark: #1d4ed8;
    --bg:          #f8fafc;
    --surface:     #ffffff;
  }

Suggest 3 alternative colour schemes for my portfolio. For each one give me:
- A name (e.g. "Forest Green", "Deep Purple")
- The 4 hex values to replace the variables above
- One sentence on what kind of impression it gives

I study [your field], so the palette should feel [adjective, e.g. "professional",
"creative", "technical"].
```

---

### Switch from a light theme to a soft dark theme

```
I have a CSS portfolio using these variables:

  :root {
    --accent:      #2563eb;
    --accent-dark: #1d4ed8;
    --bg:          #f8fafc;
    --surface:     #ffffff;
    --text:        #1e293b;
    --muted:       #64748b;
    --border:      #e2e8f0;
  }

Give me updated variable values for a soft dark theme (not pitch black —
something like GitHub's dark mode or Notion's dark mode).
Keep the same --accent blue. Show me only the updated :root block.
```

---

### Change the font

```
My portfolio uses:

  --font: 'Segoe UI', system-ui, sans-serif;

I want to use a Google Font instead. Suggest 3 font options that suit a
[your field] student portfolio. For each, give me:
1. The font name and why it works
2. The <link> tag to add to my <head>
3. The updated --font variable value

I want the font to feel [adjective, e.g. "modern and clean" / "warm and friendly" /
"technical and precise"].
```

---

## 8. Dark Mode

### Add automatic dark mode using prefers-color-scheme

```
I have a CSS portfolio with a :root block defining CSS variables for a light theme.
Here is my current :root:

[paste your :root block here]

Add a @media (prefers-color-scheme: dark) block that overrides those variables
with a dark theme. Requirements:
- Background should be around #0f172a (very dark navy)
- Surface (cards) should be around #1e293b
- Text should be near-white #f1f5f9
- Keep --accent the same blue
- Borders should be visible but subtle

Show me only the @media block to append to style.css.
No HTML changes needed — CSS variables handle everything automatically.
```

---

### Add a manual dark/light toggle button (CSS only)

```
I want a dark/light mode toggle button in my portfolio navbar.
Constraint: no JavaScript — use the CSS checkbox trick.

The toggle should:
- Look like a modern pill/switch (not a checkbox)
- Show a sun icon in light mode and a moon icon in dark mode
- Use Unicode characters for the icons (no icon library)
- Switch the :root CSS variables when checked

Show me the HTML to add to my nav, and the CSS to add to my stylesheet.
Keep it under 40 lines of CSS.
```

---

## 9. Animations

### Add a fade-in on scroll (CSS only, no JavaScript)

```
I want sections on my portfolio to fade in as the user scrolls down.
Constraint: CSS only, no JavaScript (use @keyframes + animation-timeline
or the animation-delay stagger trick).

I have section cards inside a .grid div. Each card should:
- Start invisible and slightly below its final position
- Animate into place over 0.4s with ease-out
- Stagger slightly so cards animate one after another

Show me the CSS to add to my stylesheet. If animation-timeline has poor
browser support, fall back to a simpler approach that still looks good.
```

---

### Add a hover effect to project cards

```
My project cards currently have this hover CSS:

  .card:hover { transform: translateY(-3px); box-shadow: 0 6px 18px rgba(0,0,0,.12); }

I want a more interesting hover effect. Suggest 3 options — for each show me
the CSS and describe the effect in one sentence. Requirements:
- CSS only
- Subtle and professional (this is a job-search portfolio)
- Must not break the card's layout
```

---

## 10. New Sections

### Add a blog / writing section

```
I want to add a "Writing" or "Blog" section to my portfolio.
I don't have a backend — just static HTML files.

Each post will be a separate HTML file. The section should show:
- Post title
- Date
- 1-sentence summary
- "Read more" link

Design it as a simple list (not cards) to look more like a real blog.
Show me the HTML to add to index.html and any new CSS to add to style.css.
Keep the same design language (CSS variables, same font, etc.).
```

---

### Add an "Open Source Contributions" section

```
I want to add an "Open Source" section to my portfolio showing repos I've
contributed to. It should not be a card grid — instead use a compact table or
list so I can show 6–8 items without the page looking cluttered.

Each row/item should show:
- Repo name (linked to GitHub)
- What I contributed (one line)
- Language badge (pill, same style as my existing .badge class)
- Stars count (just a number with a ★ character)

Show me the HTML and any new CSS needed.
```

---

### Add a certifications section with badge images

```
I want to add a "Certifications" section to my resume.html or skills.html.
Each certification should show:
- Certification name
- Issuing organisation
- Date earned
- (Optional) A link to verify it

I have PNG badge images saved as cert-aws.png, cert-google.png, etc.
Display them as small circular or square thumbnails next to the text.

Show me the HTML and CSS. Keep the same card / timeline style as the rest
of the page.
```

---

### Add a "Currently Reading" or "Bookshelf" section

```
I want to add a small "Currently Reading" section to my About/Home page.
It should show 2–3 book covers (images) with the title and author beneath.
Keep it minimal — no stars, no reviews.

Book cover images will be local files: book1.jpg, book2.jpg, book3.jpg.

Show me compact HTML and CSS for this section. It should look like a small
shelf, not a full-width section. Use flexbox.
```

---

## 11. Debugging & Fixes

### Fix a layout that breaks on mobile

```
My portfolio page looks fine on desktop but breaks on mobile.
Here is the problem area of my CSS:

[paste the CSS block that's causing the issue]

And here is the relevant HTML:

[paste the HTML]

The problem is: [describe what you see — e.g. "cards overflow off screen",
"nav links stack vertically and overlap the logo", "hero image is too big"]

Fix the CSS to make it work correctly on screens below 600px wide.
Explain what caused the issue and what you changed.
```

---

### Fix text that is hard to read

```
I changed my portfolio's --accent colour to [your colour].
Now some text on [light/dark] backgrounds is hard to read.

Here is my :root:

[paste :root block]

Check the contrast ratios for:
1. Body text (--text) on page background (--bg)
2. Muted text (--muted) on --bg
3. Button text (white) on --accent

WCAG AA requires 4.5:1 for normal text, 3:1 for large text.
Tell me which combinations fail and suggest fixed hex values.
```

---

### Explain a CSS rule I don't understand

```
I found this CSS in my portfolio stylesheet and I don't understand it.
Please explain it line by line, as if teaching a student who knows basic CSS
but has not seen this pattern before:

[paste the CSS rule here]
```

---

## 12. Going Further (JavaScript)

### Add a smooth scroll progress bar

```
I want to add a thin progress bar at the very top of the page (like a reading
indicator) that grows from 0% to 100% as the user scrolls down the page.

Please show me:
1. The HTML (one small div)
2. The CSS (position, colour using my --accent variable)
3. The minimal JavaScript to update the bar's width on scroll

Keep the JS under 10 lines. Vanilla JS only — no libraries.
```

---

### Add a "copy email" button

```
On my contact page I show my email address as plain text. I want to add a
small "Copy" button next to it that copies the email to the clipboard when clicked.

Show me:
1. The updated HTML for the email row
2. The CSS for the button (should match my existing .btn-outline style)
3. The minimal JavaScript (vanilla, under 10 lines) that copies the text
   and temporarily changes the button label to "Copied!"
```

---

### Add a project filter (show/hide by tech tag)

```
My projects.html has project cards, each with tech badge spans like:
  <span class="badge">Python</span>

I want to add filter buttons at the top: "All", "Python", "JavaScript", "ML"
Clicking a filter hides cards that don't include that tech badge.

Show me:
1. The HTML for the filter button row
2. The CSS
3. Vanilla JavaScript under 20 lines that handles the filtering

No jQuery. No frameworks. Explain each line of the JS.
```

---

## Tips for Getting Better Results

- **Be specific.** The more details you give (your name, your stack, your colours), the less editing you'll need to do.
- **Paste your code.** Tell the AI "here is my current HTML / CSS" before asking it to modify something.
- **Ask for explanations.** Add "explain what each line does" to any prompt — you should understand your own portfolio.
- **Iterate.** If the first answer isn't quite right, reply with "make the cards larger" or "use a softer shadow" — you don't need to start over.
- **Verify before pasting.** Read the generated code before pasting it. If something looks wrong, ask the AI to explain it.
