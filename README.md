# SLS Scholars School — Public Website

A plain HTML/CSS/JS website (no build step needed) — Home, About, Academics, Admissions, Gallery, Contact.

## Deploy to Vercel

1. Push this folder to a new GitHub repo (e.g. `sls-scholars-website`), same process as the ERP projects:
   ```bash
   cd sls-website
   git init
   git add .
   git commit -m "Initial website"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/sls-scholars-website.git
   git push -u origin main
   ```
2. On [vercel.com](https://vercel.com) → "Add New..." → "Project" → import this repo
3. Vercel will detect it as a static site — no build command needed, just deploy
4. You'll get a `.vercel.app` URL to test first

## Connect your existing domain

Once you confirm it looks right on the `.vercel.app` URL:
1. In the Vercel project → Settings → Domains → add your existing domain
2. Vercel will show you a DNS record (usually a CNAME or A record) to add
3. Log into wherever you bought the domain, go to DNS settings, add that record
4. Takes a few minutes to a few hours to propagate

## Updating content later

- Fee numbers: edit the table in `admissions.html`
- Photos: replace the emoji tiles in `gallery.html` with real `<img>` tags once you have photos
- Address/phone: edit the placeholder text in `contact.html`
- Contact form: currently opens the visitor's email app (no backend). Swap in a form service (e.g. Formspree) later if you want submissions to go somewhere more directly.
