# PHWebTech Portfolio Site

This repository hosts the marketing and portfolio pages for `PHWebTech.com`, showcasing full-stack web solutions for businesses in the Philippines.

## Project Overview
- **`index.html`**: Landing page highlighting services, experience, and directly linking to featured case studies.
- **`projects.html`**: Gallery of public-facing projects, each with imagery and descriptions.
- **`contact.html`**: Contact form and channels for prospective clients to reach the team.

All styling is handled via Tailwind CSS loaded from the official CDN, with additional imagery stored as local assets (`1.png` – `7.png`, `meta.png`).

## Getting Started
- **Serve locally**: Open `index.html` in any modern browser. No build step is required because the site is purely static.
- **Deploy**: Upload the HTML files and associated assets to your preferred static host (e.g., GitHub Pages, Netlify, or traditional shared hosting). Ensure the `meta.png` and numbered image assets remain in the same directory as the HTML files.

## Customization Tips
- **Tailwind configuration**: The inline config inside `index.html` sets project color tokens. Adjust the `tailwind.config` block if you need to extend the palette.
- **Analytics & tracking**: The site currently loads Ahrefs analytics and Google Tag Manager snippets from CDNs. Update or remove these scripts if replicating the site in another environment.
- **SEO metadata**: Modify the `<meta>` tags at the top of each page to align with your deployment domain and targeted keywords.

## Continuous Deployment
- **GitHub Pages workflow**: The workflow at `.github/workflows/gh-pages.yml` publishes the static site whenever commits land on `main` or when triggered manually. No build step is required; the action simply uploads the repository root as the deployable artifact and then runs the GitHub Pages deployment action.
- **First-time setup**: In the repository settings on GitHub, enable GitHub Pages with the "GitHub Actions" source. Subsequent pushes to `main` will update the live site automatically.

## Contributing
For tweaks or enhancements, fork the repository and open a pull request detailing the proposed change. Given the static nature of the project, keep modifications scoped and easy to verify via manual inspection.
