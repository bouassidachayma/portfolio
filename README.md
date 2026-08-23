# Chayma Bouassida — Portfolio

Personal portfolio website showcasing projects, experience, and skills as a Frontend Developer & UI/UX Designer.

🔗 **Live site:** [bouassidachayma.github.io/portfolio](https://bouassidachayma.github.io/portfolio/)

## Features

- Responsive single-page layout (desktop + mobile with collapsible nav)
- Light / dark mode toggle (saved across visits via `localStorage`)
- Scroll-reveal animations on section entry
- Project cards with a click-to-expand detail modal (full image, description, tech stack, links)
- Contact form powered by [Formspree](https://formspree.io) — no backend required
- SEO basics: meta description, Open Graph tags, JSON-LD `Person` schema
- Custom SVG favicon

## Tech Stack

- HTML5, CSS3 (custom properties for theming), vanilla JavaScript
- No build tools or frameworks — everything runs from a single `index.html`
- [Google Fonts](https://fonts.google.com) (Inter, Playfair Display)
- [Formspree](https://formspree.io) for form submissions

## Project Structure

```
├── index.html          # Main site (structure, styles, and scripts in one file)
├── favicon.svg          # Site favicon
├── photo personelle.jpg # Profile photo (rename to profile-photo.jpg, see below)
├── photo1.png            # Business Casual screenshot
├── photo2.png            # Smart Diet Planner screenshot
├── photo3.png            # Smart Workout Builder screenshot
├── photo4.png            # Personal Portfolio screenshot
├── photo5.jpg             # PayAssist AI screenshot
└── README.md
```

> **Note:** `index.html` references the profile photo as `profile-photo.jpg`. Rename your image file to match (lowercase, no spaces) before deploying, or update the `src` in the `.hero__image` section of `index.html`.

## Running Locally

No build step needed — just open `index.html` in a browser, or serve it locally:

```bash
# Python
python -m http.server 8000

# Node
npx serve .
```

Then visit `http://localhost:8000`.

## Deployment

Any static host works. Two easy free options:

**GitHub Pages**
1. Push this folder to a GitHub repo.
2. Go to Settings → Pages → set source to your main branch.
3. Your site will be live at `https://<username>.github.io/<repo-name>`.

**Netlify**
1. Drag and drop this folder into [app.netlify.com/drop](https://app.netlify.com/drop).
2. Get an instant live URL.

## Contact Form Setup

The contact form submits to Formspree. It's already connected to this project's Formspree endpoint. If you ever need to reconnect it to a different form:

1. Sign up at [formspree.io](https://formspree.io) and create a new form.
2. Copy the endpoint URL (`https://formspree.io/f/xxxxxxxx`).
3. Replace the `action` attribute on the `<form id="contactForm">` element in `index.html`.

## License

© Chayma Bouassida. All rights reserved.
