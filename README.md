# PRO-MIND Website — Fresh v2.0

Static HTML/CSS/JS site for PRO-MIND — no build tools or frameworks required. Built from your real logo, brand colors, and homepage content/design reference.

## Structure
```
├── index.html                  # Home
├── about.html                  # About Us
├── industry-experience.html
├── founder.html
├── contact.html
├── services/
│   ├── index.html               # Services overview
│   ├── business-consulting.html
│   ├── sales-transformation.html
│   ├── leadership-development.html
│   └── ai-digital-solutions.html
├── css/style.css
├── js/main.js                  # nav, animated counters, FAQ accordion, scroll reveal
├── assets/
│   ├── logo.png                 # your original uploaded logo
│   ├── logo-nav.png             # optimized version used in nav/footer
│   ├── favicon.png / favicon-512.png
├── sitemap.xml
├── robots.txt
└── .gitignore
```

## What's real vs. placeholder
**Real, already in place:**
- Your logo (nav + footer + favicon)
- Brand tagline: "Strategic Consulting. Sustainable Success."
- Real stats: 19+ years, 5000+ professionals trained, 100+ workshops, 10+ organizations
- Real contact: connectpromind@gmail.com, +91 99711 10767, WhatsApp button (bottom-right, floating)
- Real "Why PRO-MIND" 5-point copy and industry list, matching your homepage reference

**Still placeholder — replace before launch:**
- Founder page: photo, name, title, bio, philosophy, journey (`founder.html`)
- Testimonials on the home page (3 cards)
- Social links: LinkedIn, Facebook, Instagram URLs (currently `#`) — in the top bar and footer of every page
- "Download Profile" button on the homepage links to `assets/PRO-MIND-Profile.pdf`, which doesn't exist yet — either upload a real PDF profile at that path or remove the button

## Run locally
No build step — just open `index.html`, or serve it:
```
python3 -m http.server 8000
```

## Deploy on GitHub Pages
Same as before — upload all files/folders (making sure `css`, `js`, `services`, `assets` land as real folders in your repo root, not nested), then in **Settings → Pages**, set Source to your `main` branch, folder `/(root)`.

## Contact form
The form on `contact.html` currently only simulates a submission (see `js/main.js`). Connect it to a real backend — [Formspree](https://formspree.io) is the easiest no-code option — before relying on it for real leads.

## SEO
`sitemap.xml` and `robots.txt` are included and point at `https://kumaralok301.github.io/pro-mind-1/`. If you move to a custom domain, update both files and the canonical/og tags in each page's `<head>`.
