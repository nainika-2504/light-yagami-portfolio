# ✦ Light Yagami — God of the New World

> *"I am Justice. A perfect world where only I exist."*

A cinematic, single-page portfolio website themed around **Light Yagami** from Death Note. Every design decision — from the ink-black background and blood-red accents to the typewriter rules and the Death Note modal — is built to evoke the atmosphere of the anime.

---

## 🖤 Live Demo

Open `index.html` in your browser, or serve it locally:

```bash
# Any simple static server works, e.g.:
npx serve .
# then visit http://localhost:3000
```

---

## ✦ Features

| Feature | Description |
|---|---|
| **Cinematic Hero** | Split-panel hero with Light Yagami portrait, red-glow flash on hover, and a custom crosshair cursor with a trailing dot effect |
| **Interactive Image Reveal** | Hover over the right panel to trigger a red radiance overlay (canvas-based pixel reveal of Ryuk beneath Light) |
| **Typewriter Death Note Rules** | Five canonical Death Note rules typed out character-by-character as you scroll into view |
| **Judgements Grid** | Project cards styled as "case files" — hover turns the card border blood-red with an inner glow |
| **Cognitive Arsenal** | Cycling glitch-word display (`STRATEGY → JUSTICE → CONTROL → KIRA`) backed by GSAP scroll parallax |
| **Personality Profile Bars** | Animated trait bars (Intelligence 99, Ambition 95, Conviction ∞…) triggered on scroll |
| **Death Note Modal** | Click "Write a Name" to open a dramatic dark modal — enter a name, hit *Seal the Judgement*, and receive a cinematic confirmation |
| **Book-Close Animation** | Scrolling into the final section triggers a sweeping black overlay with "You have been judged." before revealing the contact CTA |
| **Film-Grain Overlay** | A subtle SVG noise texture sits at `z-index: 9999` to give the whole page an aged, paper-like feel |
| **GSAP ScrollTrigger** | Parallax on the hero text, perspective tilt on the rules section, card stagger on judgements, and red circle scale-in on the final section |

---

## 📁 File Structure

```
abb/
└── index.html      # Entire site — HTML, CSS, and JS in one self-contained file
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
