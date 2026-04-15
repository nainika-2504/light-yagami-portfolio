# ✦ Light Yagami — God of the New World

> *"I am Justice. A perfect world where only I exist."*

A cinematic, single-page portfolio website themed around **Light Yagami** from Death Note. Every design decision — from the ink-black background and blood-red accents to the typewriter rules and the Death Note modal — is built to evoke the atmosphere of the anime.

---

## 🖤 Live Demo

**[https://light-yagami-portfolio.netlify.app/](https://light-yagami-portfolio.netlify.app/)**

---

## ✦ Features

| Feature | Description |
|---|---|
| **Cinematic Hero** | Split-panel hero with portrait, red-glow flash/auto-glow, and custom crosshair cursor |
| **Mobile Simulator** | Interactive toggle to switch between Desktop and Mobile views with responsive scaling |
| **Interactive Ryuk Reveal** | Hover/erase the right panel to pixel-reveal Ryuk beneath Light using canvas rendering |
| **Judgement Execution** | Sealing a name in the Death Note triggers a cinematic, fullscreen video execution sequence |
| **Typewriter Rules** | Canonical Death Note rules typed out with GSAP-triggered perspective scroll effects |
| **Judgements Grid** | Project "case files" with blood-red glow hover states and container-query responsiveness |
| **Cognitive Arsenal** | Centered glitch-word cycling (`STRATEGY → JUSTICE → CONTROL → ...`) with scroll parallax |
| **Personality Profile** | Animated trait bars and capability grids that stack vertically on mobile/simulated views |
| **Death Note Modal** | A dramatic, book-opening modal used to capture names before the final video sequence |
| **Atmospheric Polish** | Film-grain overlay, custom scrollbars, and SVG noise textures for a premium anime feel |

---

## 📁 File Structure

```
abb/
├── index.html      # Main application logic (HTML/CSS/JS)
└── judgement.mp4   # Cinematic video asset for the judgement sequence
```

All assets (fonts, GSAP) are loaded via CDN. The portrait is embedded as a Base64 JPEG — no external image hosting required.

---

## 🎨 Design System

| Token | Value | Usage |
|---|---|---|
| `--black` | `#030303` | Page background |
| `--deep` | `#0a0a0a` | Card backgrounds |
| `--red` | `#8b0000` | Accents, borders, rule numbers |
| `--red-bright` | `#cc1111` | Hover states, glowing underlines |
| `--gold` | `#c9a84c` | Logo, hero title |
| `--white` | `#e8e0d0` | Primary text |
| `--ink` | `#d4c9a8` | Secondary text, rule text |
| `--paper` | `#1a1510` | Rules section background |

**Fonts** (Google Fonts):
- `Cinzel` — headings & logo (Roman-serif, high authority)
- `Special Elite` — typewriter / nav / caps (aged typewriter)
- `Cormorant Garamond` — body text (elegant, literary)

---

## ⚙️ Dependencies

| Library | Version | Purpose |
|---|---|---|
| [GSAP](https://greensock.com/gsap/) | 3.12.5 | ScrollTrigger parallax & card animations |
| [Google Fonts](https://fonts.google.com/) | — | Cinzel, Special Elite, Cormorant Garamond |

No build step, no bundler, no framework. Pure HTML + CSS + JS.

---

## 🗂 Sections

1. **Hero** (`#hero`) — Intro with split-panel portrait and opening quote
2. **Chronicle** (`#chronicle`) — About / backstory with hobby cards and trait bars
3. **Rules** (`#rules`) — Death Note rules typewritten on scroll, styled as a lined notebook page
4. **Judgements** (`#judgements`) — Portfolio project cards framed as "judged case files"
5. **Mind** (`#mind`) — Cognitive capabilities with glitch-word cycler
6. **Final** (`#final`) — Contact CTA with book-close animation and Death Note modal

---

## 🔧 Customisation

### Swap the portrait
Replace the `SOURCE_IMG.src` Base64 string in the `<script>` block with a URL to your own image:
```js
SOURCE_IMG.src = 'https://your-cdn.com/your-portrait.jpg';
```

### Change project cards
Edit the `.case-card` blocks inside `#judgements` — update `.case-num`, `.case-name-written`, `.case-desc`, and `.case-tag` elements.

### Update personality bars
Change `data-pct` on each `.trait-row` div to any value 0–100:
```html
<div class="trait-row" data-pct="92">
```

### Death Note rules
Edit the `data-rule` attributes on each `.rule-item` div in `#rules`.

---

## 📜 License

This project is a **creative fan portfolio** inspired by *Death Note* (© Tsugumi Ohba & Takeshi Obata / Shueisha). All original code is free to use, modify, and share.

---

<p align="center">
  <em>Death Note Portfolio — Light Yagami — The God of the New World — MMXXV</em>
</p>
