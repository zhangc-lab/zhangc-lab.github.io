# Zhang Lab — Research Website

Official website of the **Zhang Lab** at the Singapore Institute of Food and Biotechnology Innovation (SIFBI), A*STAR.

Live at: <https://zhangc-lab.github.io>

We engineer microbial cell factories — *E. coli*, yeast, fungi — for sustainable production of chemicals, fuels, and food ingredients through metabolic engineering, synthetic biology, and bioprocess optimization.

---

## Repository contents

A single self-contained static site — no build step, no dependencies.

```
zhangc-lab.github.io/
├── index.html            # Main single-page site (HTML + CSS + JS in one file)
├── join.html             # Standalone "Joining the Lab" page (linked from index.html)
├── favicon.svg           # Browser tab icon (white "Z" + DNA helix on teal)
├── logo.svg              # Lab logo for the navigation header
├── pi-headshot.webp      # PI photo (Dr. Zhang Congqiang)
├── group-photo-1.webp    # Lab gathering
├── group-photo-2.webp    # Hero / Chinese New Year celebration
├── group-photo-3.webp    # Team outing
├── figure-aucs.svg       # Research figure: AUCS expression system
├── figure-autotrophy.svg # Research figure: autotrophic pathways
├── figure-bioeconomy.svg # Research figure: C1/C2 bioeconomy
├── figure-c1c2-embedded.svg
├── figure-carotenoids.svg
├── figure-diterpenes.svg
├── figure-ionone-embedded.svg
├── figure-mhp.svg
├── figure-nerolidol-embedded.svg
└── README.md             # This file
```

## Local preview

Just open `index.html` in any modern browser. No server required.

For a closer-to-production experience (relative URL handling, etc.):

```bash
# Python 3
python3 -m http.server 8000
# Then visit http://localhost:8000
```

## Deployment

The site is deployed via **GitHub Pages** from the default branch root. To publish updates:

```bash
git add .
git commit -m "Update site content"
git push
```

GitHub Pages typically rebuilds within 1–2 minutes.

## Configuration TODO

**Optional**: replace the GitHub Pages URL with a custom domain — set up a `CNAME` file and update the `canonical`, `og:url`, `og:image`, and `twitter:image` meta tags in `index.html` and `join.html`.

## Tech notes

- **Pure static site**: HTML + CSS + vanilla JS, no frameworks, no build pipeline.
- **Fonts**: DM Sans + DM Serif Display from Google Fonts.
- **Images**: WebP for photos (small, retina-ready), SVG for figures and icons (scalable, crisp).
- **Accessibility**: semantic HTML, `aria-current` on the active carousel dot, `aria-modal` and focus management on the figure lightbox, `prefers-reduced-motion` respected on the carousel.
- **Performance**: lazy-loading on all non-hero images, optimized WebP photos, hero image hinted with `fetchpriority="high"`.
- **Social previews**: Open Graph + Twitter Card meta tags for clean LinkedIn / X / WhatsApp / Slack link previews.
- **SEO**: descriptive `<title>`, `<meta description>`, canonical URL, Google Site Verification token included.

## Sections

The site is organised as a single-page main site with one supporting sub-page.

**index.html** has six sections, all reachable via the top nav:

- **Home** — hero photo with mission statement, plus a 3-card "Recent updates" strip below the hero showing the latest publication, recruitment notice, and research highlight
- **Research** — 6 thematic areas (cell factories, biocatalysis, pathway design, omics, waste valorisation, bioprocess scale-up) plus an auto-advancing carousel of 9 selected research figures with DOIs
- **Publications & Patents** — unified chronological list (2018 – 2026) with filter tabs: All / Original Research / Reviews / Patents. The PI's name is bolded throughout. 16 papers + 11 patents = 27 entries.
- **Team** — PI profile, senior scientists, current students, alumni (former staff and former students), plus a "Life in the lab" gallery strip and a brief "We are recruiting" teaser pointing to the Join page
- **Collaborators** — primary collaborator (Dr. Chen Xixian) plus partners across Singapore, France, Germany, and China
- **Contact** — lab address, email, prospective-students note, and office hours

**join.html** is a dedicated page covering joining the lab — backgrounds we look for, scholarship pathways (AGS, ARAP, SRAP, joint NUS/NTU/SIT PhDs, postdoc fellowships), example projects, and how to apply. Linked from the recruiting teaser on the main page.

## Contact

- **Principal Investigator**: Dr. ZHANG Congqiang (Simon)
- **Email**: congqiang_zhang@a-star.edu.sg
- **Address**: Singapore Institute of Food and Biotechnology Innovation (SIFBI), 31 Biopolis Way, Nanos, Singapore 138669
- **Google Scholar**: <https://scholar.google.com/citations?user=SDgjKwIAAAAJ>
- **A*STAR Profile**: <https://research.a-star.edu.sg/researcher/congqiang-zhang/>
- **ORCID**: <https://orcid.org/0000-0003-1070-8806>
- **LinkedIn**: <https://www.linkedin.com/in/congqiang-zhang-64683791/>

---

© Zhang Lab · Singapore Institute of Food and Biotechnology Innovation (SIFBI), A*STAR
