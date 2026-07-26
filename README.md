# College Admissions Portfolio Website

This is a static, no-backend website ready for GitHub Pages.

## 1. What's in here

```
index.html              Home page
about.html               About Me
experience.html           Professional Experience
entrepreneurship.html      Bruk Kebede Legacy Project
leadership.html            Leadership roles
fellowships.html            Fellowships & Programs
awards.html                  Awards & Recognition
activities.html               Additional Activities
evidence.html                  Evidence Portfolio (full filterable gallery)
resume.html                     Online resume + PDF download
contact.html                     Contact info
css/style.css            All site styling
js/main.js                 Lightbox + gallery filter behavior
assets/img/               All evidence photos, organized by section
resume/resume.pdf         Downloadable resume (placeholder content — edit before publishing)
robots.txt                Tells search engines not to index the site (see privacy note below)
```

## 2. Before you publish — please review

I organized ~163 files from your ZIP folders using their filenames and my best judgment. Two things need your review before this goes live:

1. **`evidence.html` → "Additional Supporting Files" filter.** About 90 files (mostly `IMG_####`, undated screenshots, and email inline images) had no descriptive filename, so I couldn't confidently caption them. They're in the gallery but labeled generically. Open that filter, and for anything worth keeping, rename the file (see step 4) or just delete it from `assets/img/general/`.
2. **Placeholder personal info.** "Firstname Lastname," the email address, and the LinkedIn URL are placeholders throughout the site (nav bar, footer, `contact.html`, `resume.html`). Search each HTML file for these and replace them with your real details.
3. **`resume/resume.pdf`** has placeholder contact info too — regenerate it once you've finalized your resume content, or replace it with your own PDF (keep the filename `resume.pdf` or update the link in `resume.html`).

**Privacy note:** Once this is on GitHub Pages, the link is public — anyone who has it can view it, not only admissions officers. I added `robots.txt` and a `noindex` meta tag to every page so search engines won't index it, but that only discourages indexing, it doesn't make the page private. Don't post the link anywhere public; share it only directly with the schools you're applying to.

## 3. Uploading to GitHub Pages

1. Create a new GitHub repository (e.g. `your-username.github.io` for a root domain, or any name like `portfolio`).
2. Upload every file and folder in this project to the repository, preserving the folder structure exactly as it is here.
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment," set **Source** to "Deploy from a branch," choose the `main` branch and `/ (root)` folder, then click **Save**.
5. GitHub will give you a URL like `https://your-username.github.io/portfolio/` (or `https://your-username.github.io/` if you named the repo `your-username.github.io`). It can take a minute or two to go live.

## 4. Updating content later

- **Text:** Open any `.html` file in a text editor and edit the text directly — there's no build step, so changes are visible as soon as you push to GitHub.
- **Adding a new evidence photo:** Drop the image into the matching folder under `assets/img/` (e.g. `assets/img/awards/`), then add an entry for it in `evidence.html` (copy an existing `<div class="evidence-item">` block and update the `src`, `alt`, and caption).
- **Nav bar / footer:** These are repeated at the top and bottom of every page — if you add a new page, copy the `<header>` and `<footer>` blocks from an existing page exactly, add a new `<li><a href="...">` entry to each page's nav, and it will apply site-wide.
- **Resume PDF:** Replace `resume/resume.pdf` with an updated export from Word or Google Docs — just keep the same filename, or update the link in `resume.html`.

## 5. Design system quick reference

- Colors: Navy `#0f1e33`, gold accent `#b8912f`, paper background `#fbfaf8`
- Headings: Playfair Display (serif) — loaded from Google Fonts
- Body text: Source Sans Pro — loaded from Google Fonts
- Fully responsive; no JavaScript framework, so it loads fast on any device
