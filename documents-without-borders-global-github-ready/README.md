# Documents Without Borders Global

A complete, responsive, **static website** for Documents Without Borders Global. Built with semantic HTML5, an external stylesheet, and dependency-free JavaScript. The package contains an existing DWB conference emblem from the project materials and an original SVG illustration for the homepage.

## What's included

- Home (`index.html`)
- Mission (`mission.html`)
- Initiatives (`initiatives.html`)
- Official resources (`resources.html`)
- Global summit (`conference.html`)
- Founder (`about.html`)
- Contact (`contact.html`)
- 404 (`404.html`), SEO metadata, `robots.txt`, `sitemap.xml`, favicon
- `assets/css/styles.css` (all site styling)
- `assets/js/main.js` (responsive navigation and copyright year)
- `assets/images/` (optimized project emblem and scalable SVG brand graphics)

No build tools, package manager, framework, environment variables or paid hosting are needed. All links between pages are **relative** and therefore also work when a GitHub Pages site is hosted under a repository subpath.

## Local preview

Open `index.html` in your browser. Or, from the project folder:

```bash
python -m http.server 8000
```

Visit `http://localhost:8000`.

## Upload to GitHub (browser interface)

1. Create a new repository, for example `documents-without-borders-global`.
2. Select **Add file → Upload files** and upload **the contents of this extracted folder**, with `index.html` at the repository root. GitHub's web interface may be easier for small batches; Git CLI is recommended for preserving the directory structure.
3. Commit the files to the `main` branch.
4. Go to **Settings → Pages → Build and deployment**. Choose `Deploy from a branch`, branch `main`, folder `/ (root)`, then Save.
5. First test on the GitHub Pages address. All site navigation should work without rewriting paths.

Or use Git:

```bash
git init
git add .
git commit -m "Launch Documents Without Borders Global site"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```

Replace `YOUR-USERNAME` and `YOUR-REPOSITORY` with your actual values. This package does **not** modify any existing GitHub repo or live site.

## Connecting `documentswithoutborders.org`

The published HTML canonicals and sitemap use `https://documentswithoutborders.org/` as the intended production address. **This does not mean the domain is already pointed to the website.** Connect and verify it before requesting indexing.

For GitHub Pages: open **Settings → Pages → Custom domain**, enter `documentswithoutborders.org`, and follow GitHub's latest DNS instructions for an apex domain and optional `www` subdomain. GitHub Pages will manage or create the `CNAME` file. Enable HTTPS after DNS has settled. Do not change DNS without confirming the site should replace the current domain.

For Vercel or Netlify: import the GitHub repository. Framework: `Other` / Static. Build command: **leave empty**. Output/publish directory: **repository root (`.`)**. Attach the domain in the hosting dashboard and configure DNS exactly as your provider directs.

## Important prelaunch checks

- **Contact address:** The contact page currently uses `ceo@thenotarygiant.com` as an **interim founder contact**, not a verified DWB Global mailbox. Replace it when a dedicated address is active. Update `contact.html` (and any related visible references).
- **Legal status:** This site deliberately describes DWB Global as an educational initiative. It does not claim confirmed charitable registration, government affiliation, endorsement, board appointments or organizational status.
- **Programs and summit:** Directory, multilingual learning, country guides, Dubai summit and global conference are described as planned/concept-stage. Do not rewrite them as existing services or confirmed events until verified.
- **Legal review:** Have a qualified adviser review privacy/terms/cookie notices and entity disclosures before public launch. No personal-data collection script, cookies or analytics have been added, and there is no fabricated privacy policy.
- **Content review:** Keep official treaty sources updated. Do not publish jurisdiction-specific acceptance rules without appropriate validation.
- **Brand approvals:** The website-specific icon and illustration are original SVG artwork for this package. The conference emblem is an existing user-supplied project asset. Review logo/mark use before launch.
- **Domain:** Confirm that domain DNS, `robots.txt`, sitemap, canonical metadata and actual hosting hostname are aligned.
- **Accessibility:** Test keyboard navigation, screen readers, high contrast and major browser/mobile sizes on the eventual host.

## Maintenance

All design tokens (colors, spacing, typography), components, and responsive breakpoints are in `assets/css/styles.css`. The `main.js` file manages only the responsive menu and automatic copyright year. Static files are intentionally simple to maintain and audit.

## Attribution and disclosures

The resource page links to primary HCCH references. These links do not imply association with or endorsement by the HCCH. The project is presented as an independent educational initiative and does not provide notarizations, apostilles or legal advice through this static site.
