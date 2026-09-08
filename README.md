# Portfolio — deploy steps

This is a single-file, frontend-only site (React + Tailwind loaded via CDN, no build step, no backend).

## Deploy with GitHub Pages (simplest)
1. Create a new GitHub repo, e.g. `srija-portfolio`.
2. Add this `index.html` to the repo root and push.
3. Repo → Settings → Pages → Source: `main` branch, `/ (root)` → Save.
4. Your site goes live at `https://<username>.github.io/srija-portfolio/`.

## Deploy with GitHub + Vercel (auto redeploy on every push)
1. Push this repo to GitHub as above.
2. Go to vercel.com → New Project → Import the GitHub repo.
3. Framework preset: "Other" (no build command needed) → Deploy.
4. Every future `git push` auto-redeploys.

## Before you go live
- Replace the `#` placeholders in `PROFILE.linkedin`, `PROFILE.github`, and each project's `demo` / `code` links in `index.html`.
- Wire the contact form to Formspree (formspree.io) or EmailJS — both are free and need no backend. Update the `handleSubmit` function in `index.html` with your endpoint.
- Add a resume PDF to the repo and link it from the hero's CTA if you want a "Download Resume" button.
