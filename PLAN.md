# Scrollytelling & Decoration Enhancement Plan

## Context

The site has 10 SVG background decorations in place, but they only cover a portion of each section — leaving long stretches visually empty. Additionally, the site lacks core scrollytelling mechanics compared to the Bloomberg "What's Warming the World?" inspiration. This plan addresses both issues.

---

## Part 1: Full-Bleed SVG Decoration Tiling

**Problem**: Each SVG sits at one edge/corner of its section. Sections are tall (100–290 lines of content), so most of the vertical space has no decoration.

**Solution**: Rework each SVG to use `width: 100%; height: 100%` with `preserveAspectRatio="xMidYMid slice"` (like the HFT circuit board already does). Extend each illustration into a repeating or large-scale pattern that tiles across the full section area.

### Per-section changes:

| Section | Current | Fix |
|---|---|---|
| **Overview** (skyline) | Bottom-aligned only | Extend skyline across full width; add reflected buildings/cranes at top as a secondary row |
| **Global History** (NYSE columns) | Right side, 45% width | Expand to full-bleed; repeat column motifs across width, add subtle perspective grid floor |
| **China History** (SSE building) | Left side, 40% width | Center and scale up; add radiating concentric circles filling background |
| **China vs Global** (globes) | Centered, 90% × 80% | Already near full; add longitude/latitude grid lines extending to edges |
| **Features** (candlesticks) | Right side, 50% width | Spread candlesticks across full width; add more math symbols scattered throughout |
| **HFT** (circuit board) | Already 100% × 100% | No change needed — already the model |
| **Investing** (Great Hall) | Bottom-aligned only | Extend building wider; add seismograph line running full-width at multiple heights |
| **Access** (paifang) | Centered, 60% × 80% | Scale up to fill; add path/road lines extending from gate to edges |
| **AI** (neural network) | Right side, 42% width | Expand network to full width; add more layers and scattered nodes across left side |
| **Glossary** (bamboo scroll) | Left side, 30% width | Add multiple scrolls at different sizes; scatter small character-like marks throughout |

---

## Part 2: Full-Viewport Section Title Cards

**What**: Between major sections, insert a full-height (100vh) "chapter card" that shows just a section number, title, and a subtle decorative line. Creates breathing room and a page-turn feeling.

**Where to add** (between these section transitions):
1. Before **Overview** (after hero) — "01 / Overview"
2. Before **History** — "02 / Quantitative Hedge Fund History"
3. Before **China vs Global** — "03 / China vs. Global"
4. Before **Distinctive Features** — "04 / Distinctive Features"
5. Before **HFT** — "05 / High-Frequency Trading"
6. Before **Investing** — "06 / Investing in Chinese Quant Strategies"
7. Before **Access** — "07 / How to Access"
8. Before **AI** — "08 / Artificial Intelligence"
9. Before **Glossary** — "09 / Glossary"

**Design**:
- Full viewport height (`min-height: 100vh`)
- Centered vertically and horizontally
- Section number in large, light gold (`font-size: clamp(4rem, 8vw, 8rem)`, `opacity: 0.15`)
- Title below in white, medium weight (`font-size: clamp(1.5rem, 3vw, 2.5rem)`)
- Red-to-gold gradient divider line (60px wide, 3px tall)
- Fade-in on scroll (reuse existing `.fade-in` class)
- Background matches adjacent section's class

**CSS class**: `.chapter-card`

---

## Part 3: Sticky Charts Beside Narrative

**What**: For key chart+narrative pairs, use a two-column layout where the chart sticks (`position: sticky; top: 100px`) on one side while the narrative text scrolls past on the other side.

**Which charts to make sticky** (5 best candidates — sections with substantial narrative paired with one chart):

1. **Strategy Allocation** (China vs US doughnut charts) — `#chartStrategyCN` / `#chartStrategyUS`
   - Chart sticks left, narrative about strategy diversity scrolls right
   
2. **HFT Volume** — `#chartHFTVolume`
   - Chart sticks right, narrative about distinguishing characteristics + T+1 system scrolls left
   
3. **Quant vs Discretionary** — `#chartQuantVsDisc`
   - Chart sticks left, narrative about attractive returns + risk profile scrolls right
   
4. **Quant Quake** — `#chartQuantQuake`
   - Chart sticks right, narrative about key investment considerations scrolls left
   
5. **AI Role** — `#chartAIRole`
   - Chart sticks left, AI narrative scrolls right

**Layout**:
```
.scrolly-pair {
  display: flex;
  gap: 3rem;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 2rem;
}

.scrolly-sticky {
  flex: 1;
  position: sticky;
  top: 100px;
  align-self: flex-start;
  max-width: 500px;
}

.scrolly-narrative {
  flex: 1;
  max-width: 600px;
}
```

**Responsive**: On mobile (<900px), falls back to normal stacked layout (no sticky).

---

## Part 4: Parallax on SVG Decorations

**What**: Background SVG decorations scroll at ~50% the speed of content, creating a subtle depth/floating effect.

**Implementation**: Add a scroll event listener that applies `transform: translateY(offset)` to each `.section-bg-art` element based on how far the section has been scrolled. Use `requestAnimationFrame` for smooth 60fps performance.

```js
// Parallax on section background art
const bgArts = document.querySelectorAll('.section-bg-art');
window.addEventListener('scroll', () => {
  requestAnimationFrame(() => {
    bgArts.forEach(art => {
      const section = art.parentElement;
      const rect = section.getBoundingClientRect();
      const offset = rect.top * -0.15; // 15% parallax factor
      art.style.transform = `translateY(${offset}px)`;
    });
  });
});
```

**Factor**: 0.15 (subtle — decoration moves 15% slower than scroll). Can tune after testing.

---

## Implementation Order

1. Full-bleed decoration tiling (rework SVGs)
2. Chapter title cards (HTML + CSS)
3. Sticky chart pairs (restructure 5 sections)
4. Parallax JS (small addition)

## Files to Modify
- `index.html` — all changes in this single file

## Verification
- Open in browser, scroll full page
- Check: decorations fill sections, chapter cards create rhythm, charts stick while text scrolls, decorations float with parallax
- Check mobile (<900px): sticky falls back to stacked, chapter cards scale down
