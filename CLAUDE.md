# Clocktower Group — China Quant Deep Dive

## Project Overview

This project transforms the Clocktower Group "China Quant Deep Dive" (September 2024) research PDF into an interactive, live-hosted HTML page. The goal is a polished, dynamic single-page site that presents the research in a modern, readable web format — not a flat PDF replica, but a living document with navigation, interactivity, and visual impact.

**Hosted via GitHub Pages** on the user's personal GitHub account.

## Source Material

- **PDF location**: `research/research_article.pdf` (53 pages)
- **Author**: Clocktower Group, L.P.
- **Date**: September 2024
- **Topic**: The quantitative fund industry in China — its development, unique characteristics, investment considerations, and the role of AI

### Research Sections (from the PDF)

1. **Overview** — Executive summary of China's quant landscape
2. **Quantitative Hedge Fund History**
   - Global History (Emerging Stage pre-1980s, Rapid Growth 1980-2007, High Turbulence 2007-2008, Mature Stage post-2008)
   - China History (Emerging 2010-2015, Rapid Growth 2015-2022, High Turbulence 2023-present, What's Next?)
3. **Quant Development Stages: China vs. Global**
   - Quant Talent, Prevalence, Scale, Strategy Diversity, Trading Participation Rate, Alpha Richness, Quant Quake & Regulations, New Technology Adoption
4. **Distinctive Features**
   - Equity focus (75% of strategies), Enhanced Index Funds (EIFs), Classification & Performance of EIFs
5. **High-Frequency Trading in China**
   - Definition, T+1 Trading System, Market Making constraints, Cross-Exchange Arbitrage limitations, Tightened Leverage, Trading Speed, Intensified Regulations
6. **Investing in Chinese Quant Strategies**
   - Attractive Returns, Risks, Key Investment Considerations (Performance Consistency, AUM, Transparency, Risk Management, Reference Checks), Regulatory Risk
7. **How to Access China's Quant Strategies**
   - Onshore (QFII, RQFII), Offshore, Pros and Cons comparison
8. **Research Focus — Artificial Intelligence**
   - ML/DNN/GNN adoption, AI in investment processes, challenges
9. **Glossary** — Comprehensive definitions of quant strategies, indices, regulatory bodies, and financial instruments

### Key Data Points for Visualization

- China quant AUM growth: 3% (2016) to 27% (2023Q3) of hedge fund AUM
- Strategy allocation: China (75% equity) vs. U.S. (35% CTA, 25% macro)
- Top 10 quant funds comparison: China ($55B combined) vs. Global ($735B combined) — 13x gap
- EIF annual median alpha: ~11% (CSI 300), ~13% (CSI 500), ~17% (CSI 1000) from 2020-2023
- Quant trading participation: 20-30% of Chinese equity volume vs. 58% in U.S.
- HFT volume: ~20% in China vs. ~50% in U.S.
- CSI index comparisons (300, 500, 1000, 2000): volatility, correlation, market cap distribution
- Feb 2024 "Quant Quake": top managers saw -18% alpha drawdown in one week
- Onshore vs. Offshore access: fees, latency, trading days, leverage, FX impact

## Technical Approach

### Stack
- **Single HTML file** with embedded CSS and JS (no build step, easy to host)
- Modern CSS (Grid, Flexbox, CSS custom properties for theming)
- Vanilla JS for interactivity (no framework dependencies)
- Charts via a lightweight library (Chart.js or similar, loaded via CDN)
- Responsive design (desktop-first, mobile-friendly)

### Design Direction — Scrollytelling

**Inspiration**: Bloomberg's "What's Warming the World?" interactive article.
**Format**: Scrollytelling — sticky visuals/charts stay pinned while narrative text scrolls past. Each scroll step reveals new data, transitions, or context.

**Key UX Patterns**:
- `position: sticky` for pinned charts/visuals alongside scrolling narrative
- Intersection Observer API for scroll-triggered animations and data reveals
- Full-viewport hero and section transitions
- Progressive data revelation — charts build up as the reader scrolls
- Smooth CSS transitions between states
- Optional progress indicator (thin bar at top)

**Color Palette** — China flag-inspired:
- Deep red-black backgrounds (`#1a0a0a`, `#2a0f0f`) for dark sections
- Red accents: `#c62828` (primary), `#8b0000` (dark), `#ef5350` (light)
- Gold accents: `#d4a017` (primary), `#ffd54f` (light), `#a67c00` (dark)
- Warm grays (`#8b7070`, `#d4c4c4`) instead of cool/blue grays
- High contrast for readability
- Chart colors use red and gold tones to stay on-palette

**Typography**:
- All text uses `Calibri` (system font) — no Google Fonts, no serifs
- Strong size hierarchy via weight and size for scrollytelling impact

**Logo**: Official Clocktower Group logo PNG (`assets/ctg_logo.png`) — black on white original, CSS `filter: invert(1)` for dark backgrounds. Used in nav, hero intro, and footer.

**Hero — Scroll-to-Expand Animation** (from `example_components/component_2.md`, converted to vanilla JS):
- A centered media rectangle (340×420 on desktop, 280×380 on mobile) sits over a darkened China flag background (`assets/China_flag.png`, `brightness(0.25) saturate(0.8)`)
- Wheel/touch events are intercepted; `scrollProgress` goes from 0 → 1 as the user scrolls
- The rectangle expands to fill the full viewport, border-radius shrinks to 0, box-shadow fades out
- The split title ("China" / "Quant Deep Dive") translates apart (left/right) as progress increases
- Subtitle, meta info, and scroll indicator fade out quickly
- The Clocktower logo inside the media starts invisible and fades in as the user scrolls
- Once `scrollProgress >= 1`, normal page scrolling resumes (`mediaFullyExpanded = true`)
- Scrolling back up from the top (`scrollY <= 5`) reverses the expansion
- An entropy particle animation (canvas, from `example_components/component_1.md`) renders inside the expanding media — canvas is initialized at viewport size, centered with `transform: translate(-50%, -50%)`, and clipped by `overflow: hidden` on the container so more is revealed as it expands. Particle count is capped at 600 for performance; connection lines are only drawn when particle count is under 400.

### File Structure
```
clocktower_group/
├── CLAUDE.md                  # This file — project context
├── index.html                 # The main deliverable — the live page
├── research/
│   └── research_article.pdf   # Source PDF (53 pages)
├── assets/
│   ├── China_flag.png         # Hero background image
│   └── ctg_logo.png          # Clocktower Group logo (black on white)
├── example_components/
│   ├── component_1.md        # Entropy animation reference component
│   └── component_2.md        # Scroll-to-expand media reference component
└── website_screenshot/
    └── www.clocktowergroup.com_ (1).png  # Brand reference screenshot
```

### Deployment
- **GitHub repo**: https://github.com/AugustineCarB/ctg
- Enable GitHub Pages (serve from `main` branch root)
- The `index.html` file becomes the live site at `augustinecarb.github.io/ctg`

## Design Principles

1. **Faithful to the research** — all substantive content from the PDF should be represented
2. **Better than the PDF** — interactive charts, smooth navigation, responsive layout
3. **Self-contained** — single HTML file, CDN-loaded dependencies only
4. **Professional** — this represents Clocktower Group's research quality
5. **Accessible** — proper semantic HTML, readable typography, good contrast

## Important Notes

- The PDF contains proprietary Clocktower Group research with a disclaimer. The HTML page should include the disclaimer section.
- Charts and data visualizations should be recreated from the data in the PDF, not embedded as images.
- The Clocktower Group logo/branding should be represented in the header.
- Do NOT use any external context about Bitcoin layers or crypto — only content from the PDF itself.

## CRITICAL — Content Fidelity Rule

**DO NOT summarize, paraphrase, shorten, or rephrase any text from the PDF.** Every sentence, paragraph, bullet point, and data point must be copied verbatim from the source PDF. The HTML page is a faithful reproduction of the research document — not an interpretation or summary of it. If a paragraph in the PDF has 5 sentences, the HTML must have those exact 5 sentences with the exact same wording. Do not omit sentences, combine paragraphs, round numbers differently, or reorganize content. When in doubt, re-read the specific PDF page and copy the text exactly as written.

## Current Status

- [x] PDF read and analyzed (all 53 pages)
- [x] CLAUDE.md created
- [x] index.html — initial scaffold with scrollytelling layout
- [x] Section-by-section content (Overview, History, China vs Global, EIFs, HFT, Investing, AI)
- [x] Data visualizations — 4 Chart.js charts (strategy mix, EIF alpha, HFT volume, AI adoption)
- [x] Navigation (fixed top bar with section links, progress bar)
- [x] Scroll animations (Intersection Observer fade-ins, scrolly steps, timeline)
- [x] Entropy particle animation on hero (from component 1)
- [x] Scroll-to-expand hero animation (from component 2) — media rectangle expands to viewport on scroll, title splits apart, logo fades in
- [x] China flag background on hero
- [x] Clocktower Group logo integrated (nav, hero expanding media, footer)
- [x] Color palette: China flag-inspired reds and golds (no blues)
- [x] Typography: all Calibri, no serifs
- [x] Content fidelity pass — 7 sections cross-referenced with PDF and corrected verbatim (EIFs, HFT, T+1, Market Making, Trading Speed, Regulatory Risk, Glossary + Disclaimer)
- [ ] Responsive design polish
- [ ] GitHub repo setup and deployment
- [ ] Additional content sections or refinements as needed
