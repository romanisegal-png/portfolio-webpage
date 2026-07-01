# Portfolio Webpage — Project Notes

**Owner:** Roman Segal  
**Program:** M.L.S. in Cybersecurity Law & Policy, Texas A&M School of Law  
**Live Site:** https://portfolio-webpage-mu-two.vercel.app  
**GitHub Repo:** https://github.com/romanisegal-png/portfolio-webpage  
**Vercel Project:** https://vercel.com/roman-segal-s-projects/portfolio-webpage

---

## Repository Structure

```
portfolio-webpage/
├── index.html              # Main portfolio page
├── vercel.json             # Vercel config (cleanUrls, trailingSlash)
├── README.md               # Short repo description
├── PROJECT_NOTES.md        # This file — workflow reference
└── papers/
    └── mpdpa-research-paper.pdf   # MPDPA research paper
```

---

## Deployment Workflow

This project uses **GitHub → Vercel auto-deploy**.

- Every commit pushed to the `main` branch automatically triggers a new Production deployment on Vercel.
- No manual steps needed after committing.

---

## How to Add a New Paper

1. Go to **GitHub → portfolio-webpage → papers/**
2. Click **Add file → Upload files**
3. Upload your PDF (use a clean filename, e.g. `data-breach-paper.pdf`)
4. Commit directly to `main`
5. Open `index.html`, find the relevant Core Coursework section, and add a link:
   ```html
   <a href="papers/data-breach-paper.pdf" target="_blank">View Paper</a>
   ```
6. Commit the updated `index.html` — Vercel will auto-deploy within ~30 seconds

---

## How to Edit the Portfolio Page

1. Go to **GitHub → portfolio-webpage → index.html**
2. Click the **pencil icon** (Edit this file)
3. Make your changes
4. Click **Commit changes** → Commit directly to `main`
5. Vercel auto-deploys the updated site

---

## How to Return to This Project Later

- **GitHub:** https://github.com/romanisegal-png/portfolio-webpage
- **Vercel Dashboard:** https://vercel.com/roman-segal-s-projects/portfolio-webpage
- **Live Site:** https://portfolio-webpage-mu-two.vercel.app

---

## Future To-Do Ideas

- [ ] Add remaining core coursework sections as courses are completed
- [ ] Upload additional research papers to `papers/`
- [ ] Add a custom domain (e.g. `romansegal.com`)
- [ ] Add a contact or LinkedIn section
- [ ] Consider a `development` branch for drafting changes before publishing

---

## vercel.json Reference

```json
{
  "cleanUrls": true,
  "trailingSlash": false
}
```
