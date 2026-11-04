# Waleed Ahmed | AI Engineer Portfolio

A one-page personal portfolio for **Waleed Ahmed**, an AI Engineer based in Karachi, Pakistan, who builds AI agents and automations that ship.

![Portfolio preview](screenshot-desktop-hero.png)

## About

I work as the in-house AI Engineer at **Sygnea Digital**, a performance marketing agency, where I've built and deployed 15+ AI agents and automations, including lead-qualification agents that made lead qualification 40% more efficient. As an AI Trainer with **Apna Kamao** (150K+ audience), I created an 11+ hour AI & Vibe Coding workshop that takes beginners from zero to building their own software with AI.

## Features

- **Interactive 3D hero:** a Three.js neural-network particle sphere that reacts to mouse movement and scrolling
- **Scroll animations:** GSAP ScrollTrigger reveals, a timeline progress line, and animated stat counters
- **3D tilt cards** with a light glare that follows the cursor
- **60/30/10 color system:** near-black background, white text, and a single lime accent (`#CEF432`) used only on the main call-to-action buttons
- **Typography:** Clash Display for headlines and Satoshi for body text, both from Fontshare
- **Workshop section** with a lightweight click-to-play YouTube embed (privacy-friendly `youtube-nocookie.com`)
- **Responsive and accessible:** a mobile menu, fewer particles on phones, `prefers-reduced-motion` support, and a static fallback when WebGL isn't available
- **A single self-contained file:** all CSS, JS, and the photo are inside `index.html`

## Tech Stack

| Area | Tools |
| --- | --- |
| Markup and styles | HTML5, CSS3 (custom properties, grid, flexbox) |
| 3D | [Three.js](https://threejs.org/) r160, loaded as an ES module from a CDN |
| Animation | [GSAP](https://gsap.com/) 3.12.5 with ScrollTrigger |
| Fonts | [Fontshare](https://www.fontshare.com/) (Clash Display, Satoshi) |

## Project Structure

```
.
├── index.html          # The whole site (inline CSS/JS, embedded photo)
├── waleed-photo.webp   # Profile photo, used for social link previews (og:image)
├── screenshot-*.png    # Preview images for this README
└── README.md
```

## Run Locally

No build step is needed. Serve the folder with any static server so the YouTube embed works:

```bash
# Python
python3 -m http.server 8000

# or Node
npx serve .
```

Then open http://localhost:8000. Opening `index.html` directly from disk also works, but the workshop video will open on YouTube instead of playing inline.

## Deploy

**GitHub Pages**
1. Push these files to a repository (for example `waleed-portfolio`).
2. Go to **Settings > Pages**, set the source to **Deploy from a branch**, then pick `main` and `/ (root)`.
3. Your site goes live at `https://<your-username>.github.io/<repo-name>/`.

**Netlify or Vercel:** import the repo, or drag the folder into [Netlify Drop](https://app.netlify.com/drop). No build command or output folder is needed.

After deploying, update the `og:image` and `og:url` meta tags in `index.html` to your live URL so link previews show your photo.

## Customize

- **Colors:** edit the CSS variables at the top of the `<style>` block in `index.html`.
- **Content:** every section is plain HTML with clear `id`s (`about`, `highlights`, `workshop`, `experience`, `skills`, `education`, `contact`).
- **3D scene:** particle counts and colors are set near the top of the Three.js module script.

## Contact

- Email: [waleed007896@gmail.com](mailto:waleed007896@gmail.com)
- LinkedIn: [linkedin.com/in/waleed-ai](https://www.linkedin.com/in/waleed-ai)
- WhatsApp: [+92 308 2112124](https://wa.me/923082112124)
- Instagram: [@aiwithwaleed](https://www.instagram.com/aiwithwaleed/)
- Facebook: [WaleedTheDev](https://www.facebook.com/WaleedTheDev)
- Workshop: [AI & Vibe Coding Bootcamp on YouTube](https://www.youtube.com/watch?v=gqfp1O4vAgI&list=PLdsUEmlhUIjU)

---

© 2026 Waleed Ahmed. Built with Three.js and GSAP.
