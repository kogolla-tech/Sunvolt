# SUNVOLT.AFRICA Website

Responsive, dependency-free static website built with HTML, CSS and vanilla JavaScript.

## Project structure
- `index.html` — website content and page structure
- `assets/css/styles.css` — responsive visual system
- `assets/js/main.js` — mobile navigation, year and enquiry handoff
- `assets/favicon.svg` — browser icon
- `.github/workflows/deploy-pages.yml` — automatic GitHub Pages deployment
- `.github/ISSUE_TEMPLATE/` — bug and feature issue templates
- `.github/PULL_REQUEST_TEMPLATE.md` — pull request checklist

## Run locally
Open `index.html` in a browser, or run `python -m http.server 8000` from the repository root and visit `http://localhost:8000`.

## GitHub setup
1. Create a GitHub repository, e.g. `sunvolt-africa`.
2. Push the contents of this folder to the repository's `main` branch.
3. In repository **Settings → Pages**, set the source to **GitHub Actions**.
4. Push to `main`. The included workflow deploys the static site.
5. Check the **Actions** tab and Pages settings for the deployment URL.

## Custom domain
To use `sunvolt.africa`, first confirm domain registration and DNS control. In **Settings → Pages**, add the custom domain and configure the DNS records GitHub specifies. Rename `CNAME.example` to `CNAME` and ensure its only content is `sunvolt.africa`. Verify DNS in GitHub before enabling HTTPS. Do not assume the domain is registered or configured.

## Contact form limitation
The form currently creates a `mailto:` enquiry and opens the visitor's email application. It does not submit to a server, save data or connect to a CRM. Confirm `hello@sunvolt.africa` is an approved contact address before launch. For a hosted form, select and configure a backend or CRM and publish an appropriate privacy notice.

## Before launch
Confirm the official legal/trading name, email, phone, address, domain ownership, service descriptions, technical qualifications, licences, warranties and customer permissions. Add approved project photography and genuine testimonials. Test all links and layouts on mobile and desktop.

## Suggested Git workflow
Use `main` for production. Create `feature/<description>` and `fix/<description>` branches, test locally, commit focused changes, open a pull request and merge after review. Example commits: `feat: add solar case study`, `fix: improve mobile menu`, `docs: update contact details`.
