Broad-based Index EIFs Performance Comparison section is a bit off. Some sentences are cut off and others are not even there. 
High frequency trading in China section also has some off sentences. 
T+1 Trading section is also off. 
China’s Markets Are Not Conducive to Market Making or Cross-Exchange Arbitrage Strategies section is also off. 
Trading Speed Improvement is Less Frenzied section is also off
Regulatory risk section is also off
Key Terms and Definitions section is also off


---

## Timeline Discrepancies: Global History (index.html vs PDF)

The "History of Global Quant Development" timeline graphic (PDF p.2) has different bullet points than what's shown in the HTML timeline (index.html lines 1096–1158).

### Emerging Stage (Pre-1980s)
- **PDF graphic bullets:**
  - Modern Portfolio Theory
  - Efficient Market Hypothesis
  - Option Pricing Theory
  - 1969, first quant fund, PNP
  - 1971, first passive quant fund
- **HTML timeline bullets:**
  - Modern Portfolio Theory, Efficient Market Hypothesis, Option Pricing Theory *(combined into one bullet)*
  - 1969: First quant fund (Princeton Newport Partners)
  - 1971: First passive quant fund (Barclays)
- **Differences:** PDF lists the three theories as separate bullets; HTML combines them into one. Otherwise content matches.

### Rapid Growth (1980–2007)
- **PDF graphic bullets:**
  - Rapid AUM growth: ~10B USD in 1989 to ~400B USD in 2007
  - Advancements in computer tech
  - Policy support
  - Late 80s: statistical arbitrage, trend following strategies
  - After the 90s: multi-factor models and algorithmic trading
- **HTML timeline bullets:**
  - AUM grew from ~$108B (1989) to ~$400B (2007)
  - Advancements in computer technology & electronic trading
  - Statistical arbitrage, trend following, multi-factor models
  - Key firms: Renaissance, D.E. Shaw, Citadel, Two Sigma
- **Differences:**
  1. AUM starting figure: PDF says "~10B" but HTML says "~$108B" — need to verify which is correct from the PDF body text (body text on p.3 says "$400 billion" for 2007 but doesn't give the 1989 figure in the same sentence; the graphic says ~10B)
  2. PDF has "Policy support" bullet — HTML is missing this entirely
  3. PDF splits strategies by decade ("Late 80s" / "After the 90s") — HTML combines them
  4. PDF does NOT have "Key firms: Renaissance, D.E. Shaw, Citadel, Two Sigma" — HTML added this (the PDF body text mentions Renaissance and D.E. Shaw but the graphic itself does not list key firms as a bullet)

### High Turbulence (2007–2008)
- **PDF graphic bullets:**
  - Aug 2007 - quant quake
  - 2008 - financial crisis
- **HTML timeline bullets:**
  - Aug 2007: Quant Quake — losses of 5%–30%
  - 2008: Global financial crisis, AUM shrank ~20%
  - Citadel flagship funds saw 55% drawdown
  - Medallion Fund posted +80% return in 2008
- **Differences:**
  1. PDF graphic only has 2 bullets; HTML has 4 bullets
  2. HTML added detail from the body text (loss percentages, AUM shrinkage, Citadel drawdown, Medallion return) that is NOT in the timeline graphic itself
  3. The graphic is intentionally brief — HTML should match the graphic's brevity

### Mature Stage (Post 2008)
- **PDF graphic bullets:**
  - Stricter regulations & enhanced risk management: Dodd-Frank
  - Alternative data and AI
  - Smart beta
  - Renaissance, AQR, Two Sigma are all over 50B USD
- **HTML timeline bullets:**
  - Stricter regulations & enhanced risk management
  - Dodd-Frank Act (2010)
  - Alternative data & AI adoption
  - Renaissance, AQR, Two Sigma each exceed $50B AUM
- **Differences:**
  1. PDF combines "Stricter regulations & enhanced risk management: Dodd-Frank" as one bullet — HTML splits this into two separate bullets
  2. PDF has "Smart beta" as its own bullet — HTML is MISSING "Smart beta" entirely
  3. PDF says "are all over 50B USD" — HTML says "each exceed $50B AUM" (minor wording difference but should match the graphic)

---

## Timeline Discrepancies: China History (index.html vs PDF)

The "History of China Quant Development" timeline graphic (PDF p.5) vs HTML timeline (index.html lines 1233–1294).

### Emerging Stage (2010–2015)
- **PDF graphic bullets:**
  - April 2010: Launch of CSI 300 Index Futures (IF), providing short instrument
  - Quant Market-Neutral strategies grew rapidly with sizing factor continuously contributing
  - Most models built around multi-factor frameworks
- **HTML timeline bullets:**
  - April 2010: Launch of CSI 300 Index Futures (IF)
  - Quant market-neutral strategies grew rapidly
  - Size factor continuously contributing alpha
  - Most models built around multi-factor frameworks
- **Differences:**
  1. PDF's first bullet includes "providing short instrument" — HTML cuts this off
  2. PDF combines quant MN strategies + sizing factor into one bullet — HTML splits into two separate bullets
  3. HTML adds the word "alpha" after "contributing" — PDF just says "continuously contributing"

### Rapid Growth (2015–2022)
- **PDF graphic bullets:**
  - AUM Rapid Growth: ~$13B in 2015 to ~$214B in 2022
  - April 2015: Launch of SSE 50 and CSI 500 Index Futures
  - Quant products quickly evolved – from MN to EIF to multi-strategy
  - Quant strategies transitioned rapidly – from higher to lower frequency, incorporating alternative data, ML & AI.
- **HTML timeline bullets:**
  - AUM grew from ~$13B (2015) to ~$214B (2022)
  - April 2015: Launch of SSE 50 & CSI 500 Index Futures
  - Products evolved from MN to EIF to multi-strategy
  - Transition from higher to lower frequency; ML & AI adoption
- **Differences:**
  1. PDF says "AUM Rapid Growth:" — HTML just says "AUM grew from"
  2. PDF's last bullet mentions "incorporating alternative data" — HTML drops "alternative data" and just says "ML & AI adoption"

### High Turbulence (2023–Present)
- **PDF graphic bullets:**
  - Beginning in early 2023, a series of regulations were issued regarding the quant industry.
  - In February 2024, the "Quant Quake" hit. During the week of February 8th, top quant funds saw their CSI 500 Enhanced Indexing Fund suffer average alpha drawdowns of around 9%.
- **HTML timeline bullets:**
  - Series of regulations issued targeting quant industry
  - Feb 2024: "Quant Quake" hit China
  - Top quants' CSI 500 EIFs saw ~9% avg alpha drawdown in one week
- **Differences:**
  1. PDF's first bullet starts with "Beginning in early 2023" — HTML drops the time reference
  2. PDF combines the Quant Quake date and the drawdown detail into one bullet — HTML splits into two bullets
  3. Minor wording simplifications throughout

### Mature Stage – Future ("What's Next?")
- **PDF graphic bullets:**
  - Tight regulations on the quant space will become a norm
  - Industry consolidation – big funds will become bigger
  - Winner takes all – who survived from the last rounds
- **HTML timeline bullets:**
  - Tight regulations on quant space will become the norm
  - Industry consolidation — big funds will become bigger
  - Winner takes all: survival of the most resilient
- **Differences:**
  1. PDF says "become a norm" — HTML says "become the norm" (minor)
  2. PDF says "who survived from the last rounds" — HTML rephrases to "survival of the most resilient" (should match PDF verbatim)

---

---

## Foreign Languages Spoken Pie Chart (Right side of Demographics section)

The "Foreign Languages Spoken" donut chart in the HTML has wrong data. Per the PDF (source: ZIPPIA):
- **51% Chinese** (HTML may have wrong value)
- **9% Spanish** (HTML may have wrong value)
- **7% Japanese** (HTML may have wrong value)
- **33% Other** (HTML may have wrong value)

Need to verify the actual values in the chart JS code and correct them to match these exact percentages.

---

## Global Quantitative Hedge Funds AUM ($bn) Stacked Bar Chart

Two issues found comparing HTML chart vs PDF chart:

1. **Wrong percentage label for 2011 and 2012:**
   - HTML shows 2011 as 28% — should be **25%**
   - HTML shows 2012 as 28% — confirm this is correct (PDF shows 28% for 2012)
   - Need to fix the 2011 percentage value in the JS data

2. **2007 bar should be taller than 2008 bar:**
   - In the PDF, the 2007 total bar is visibly higher than 2008 (AUM shrank ~20% during the financial crisis)
   - In the HTML, 2008 appears equal or taller than 2007 — the underlying data values for total AUM in 2007 and 2008 need to be checked and corrected so 2007 > 2008

---

## China Quant Rapid Development Chart — COMPLETELY WRONG

The HTML chart is fundamentally different from the PDF chart. Needs to be rebuilt from scratch.

**PDF chart structure:**
- **Chart type:** Grouped bar chart (side-by-side bars) with a line overlay
- **Three data series:**
  1. Discretionary Fund AUM (USD bn) — gray bars
  2. Quant Fund AUM (USD bn) — purple/magenta bars
  3. Cum No of Quant LOs Launched since 2016 — shown as stacked/overlay on the bars (dark blue)
- **Percentage labels** on top of each year group showing quant's share: 3%, 6%, 8%, 17%, 19%, 24%, 27%, 27%
- **Two Y-axes:** Left = AUM (USD bn), Right = No. of Funds
- **Years:** 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023Q3
- **Source:** CICC AM, CITIC Securities, AMAC, simuwang.com

**HTML chart (current — wrong):**
- Shows Discretionary AUM as tall gray bars and Quant AUM as short red bars (side-by-side) with a gold line for cumulative launches
- The bar proportions, chart type, and visual structure are all different from the PDF
- The Discretionary AUM bars in HTML are way too tall (~500+ range) compared to the PDF (~400–1100 range for total)
- Missing the percentage labels on top of each year group
- The overall visual does not match the PDF at all

**Action:** Rebuild this chart entirely to match the PDF's grouped bar structure, data values, and percentage annotations.

---

## Low Concentration of China Quants Pie Chart — Labels Wrong

The HTML shows percentage labels (5%, 6%, 7%, 9%, 70%) but the PDF shows **nominal number of firms** as labels:
- >10bn RMB: **32**
- 5-10bn RMB: **23**
- 2-5bn RMB: **40**
- 1-2bn RMB: **51**
- 500mn-1bn RMB: **63**
- <500mn RMB: **480**

**Action:** Change the chart labels from percentages to the actual number of firms (32, 23, 40, 51, 63, 480). The chart is a standard pie (not donut) in the PDF, but donut style is fine — just fix the labels to show counts, not percentages.

---

## Top 10 Quant Funds AUM Comparison Chart — COMPLETELY WRONG

The HTML shows a simple horizontal bar chart with just two bars (China $55B, Global $735B). The PDF is a much more detailed stacked/labeled vertical bar chart.

**PDF chart structure:**
- **Vertical stacked bar chart** with two columns: "China Top 10" and "Global Top 10"
- **China Top 10 bar** ($55B total) — small bar with individual fund names listed beside it:
  - Minghong, 8
  - Ubiquant, 8
  - Yanfu, 8
  - Lingjun, 7
  - Chengqi, 6
  - Wizardquant, 5
  - Century Frontier, 4
  - High-Flyer, 4
  - Wenbo, 3
  - Tianyan, 3
- **Global Top 10 bar** ($735B total) — tall stacked bar with each fund as a labeled segment:
  - Man, 178
  - Renaissance, 106
  - AQR, 95
  - Squarepoint, 76
  - Two Sigma, 67
  - Marshall Wace, 64
  - Citadel, 52
  - D.E. Shaw, 46
  - PanAgora, 32
  - DBi, 20 (partially visible)
- **"13x" annotation** with an arrow between the two bars showing the gap
- Y-axis: Billion USD (0–800)

**HTML chart (current — wrong):**
- Just two plain horizontal bars, no individual fund breakdown
- No stacked segments, no fund names, no 13x arrow annotation
- Completely different orientation (horizontal vs vertical)

**Action:** Rebuild this chart as a vertical stacked bar chart with individual fund segments labeled, matching the PDF layout. Include the "13x" annotation.

---

## China Quant Strategy Allocation by AUM Pie Chart — Wrong Percentages

The HTML has some values swapped/wrong. Correct values per PDF:
- Equity Enhanced Index Fund (EIF, Long-Only): **39%** (HTML correct)
- Equity Market Neutral: **33%** (HTML correct)
- CTA: **9%** (HTML may have this swapped with Equity L/S)
- Equity L/S & Equity Index-Free EIF: **8%** (HTML may have this swapped with CTA)
- Quant Macro: **5%** (check HTML)
- Multi-strategy: **4%** (HTML may be wrong)
- Stat Arb: **3%** (HTML may be wrong)

**Action:** Fix the data values so CTA=9%, Equity L/S=8%, Stat Arb=3%, Multi-strategy=4%. Verify Quant Macro=5%.

---

## China Quant EIFs Annual Alpha vs U.S. Quant EMN Chart — Legend Labels

The legend labels in the HTML are missing the word "Median". Per the PDF:
- "300 EIF Median Alpha" (HTML currently says "CSI 300 EIF Alpha")
- "500 EIF Median Alpha" (HTML currently says "CSI 500 EIF Alpha")
- "1000 EIF Median Alpha" (HTML currently says "CSI 1000 EIF Alpha")
- "US Quant EMN Return" (this one is fine)

**Action:** Add "Median" to the first three legend labels to match the PDF.

---

## Quant Institutions' Research Coverage Chart — Title/Subtitle Flipped

In the PDF:
- **Title:** "A-shares & Futures Are The Main Investment Research Focus in China"
- **Subtitle:** "Quant Institutions' Research Coverage in Asset Class"

In the HTML these are reversed:
- **Title (currently):** "Quant Institutions' Research Coverage in Asset Class"
- **Subtitle (currently):** "A-shares & Futures Are The Main Investment Research Focus in China"

**Action:** Swap the title and subtitle so they match the PDF order.

---

## Barra Factor Cumulative Returns Chart — Replace with Screenshot

This chart is too intricate to recreate with Chart.js (10 line series with detailed time-series data we don't have). Instead of the current generated chart:

1. **Replace with a screenshot** from `assets/charts/` folder (need to identify which page has this chart — likely around page 14-16 of the PDF)
2. **Add a scroll-triggered animation:** As the user scrolls down, the chart image fades/slides into view. As they keep scrolling past it, it fades/slides out.
3. Remove the current Chart.js canvas for this chart entirely.

**Action:** Find the correct page screenshot, replace the chart with an `<img>` tag, and add Intersection Observer-based fade-in/fade-out scroll effect.

---

## EIFs Breakdown Chart — COMPLETELY WRONG

The HTML shows two donut charts side by side. The PDF shows a completely different layout: one pie chart + one stacked bar.

**PDF chart structure:**
- **Title:** "Broad-based Index EIFs are Dominant & The CSI 500 EIF is Mainstream"
- **Subtitle:** "EIFs Breakdown (by number of products)"
- **Left side:** Pie chart (not donut) with labels inside the slices:
  - Broad-based Index, 65%
  - Index-Free EIFs, 29%
  - Other Index, 6%
- **Right side:** Stacked vertical bar (NOT a second pie/donut) breaking down the 65% Broad-based Index:
  - CSI 500, 45%
  - CSI 1000, 13%
  - CSI 300, 6%
  - Others, 1%
- **Source:** Simupaipai as of July 2023. China Quant Investment Quarterly Report – 2023 Fall.

**HTML chart (current — wrong):**
- Shows two donut charts side by side
- Right donut has wrong values: 69%, 20%, 9% (should be 45%, 13%, 6%, 1%)
- Right side should be a stacked bar, not a donut
- Title/subtitle are flipped (same issue as the Research Coverage chart)

**Action:** Rebuild entirely. Left side stays as a pie/donut with correct values. Right side should be a stacked vertical bar chart showing CSI 500=45%, CSI 1000=13%, CSI 300=6%, Others=1%. Fix the title/subtitle order.

---

## High Frequency Trading Definitions Table — COMPLETELY WRONG CONTENT

The HTML table is heavily summarized/shortened. The PDF has full verbatim bullet points for each regulator. Need to replace with exact PDF text.

**PDF table content (verbatim):**

**U.S. CFTC:**
- Algorithms for decision making, order initiation, generation, routing, or execution, for each individual transaction without human direction.
- Low-latency technology that is designed to minimize response times, including proximity and co-location services.
- High speed connections to markets for order entry.
- High message rates (orders, quotes or cancellations)

**U.S. SEC:**
- Use of extraordinarily high speed and sophisticated programs for generating, routing, and executing orders.
- Use of co-location services and individual data feeds offered by exchanges and others to minimize network and other latencies.
- Very short time-frames for establishing and liquidating positions.
- Submission of numerous orders that are cancelled shortly after submission.
- Ending the trading day in as close to a flat position as possible.

**China CSRC:**
- HFT is a type of algorithmic trading involving a high number and frequency of order submissions and cancellations within a short period.
- Specifically, order submission and cancellation over 300 orders per second or over 20,000 orders per day.

**HTML table (current — wrong):**
- Condensed each regulator's definition into 1-2 sentences instead of full bullet lists
- Missing multiple bullet points from CFTC and SEC definitions
- Column headers say "Regulator" / "Definition / Criteria" — PDF says "Source" / "Definition"

**Action:** Replace the HTML table content with the exact verbatim bullet points from the PDF for each regulator. Fix column headers to match PDF.

---

## Trading Systems Overview Table — COMPLETELY WRONG CONTENT

The HTML table is heavily simplified. The PDF table spans two pages (p.23-24) with detailed, multi-paragraph content for each cell. The HTML has short 1-sentence summaries instead.

**Key differences by row:**

**Definition row:**
- PDF China column has extensive detail: explains continuous auction, batch auction, Shenzhen Stock Exchange schedule with specific times (Opening batch auction: 9:15–9:25, Continuous auction sessions: 9:30–11:30 and 13:00–14:57, Closing batch auction: 14:57–15:00)
- HTML just says "Orders matched directly based on price and time priority among investors through a centralized process"

**Primary Profit Mechanism row:**
- PDF says "No dedicated market-making profiting mechanism" (China) and "Market makers can profit from bid-ask spreads, exchange rebates and trade execution advantages" (U.S.)
- HTML has different wording: "No exchange rebates; no market maker required" / "Exchange rebates and bid-ask spread capture"

**Transparency row:**
- PDF has detailed text about information being publicly available, buyer/seller quotes, transaction details (China); and "Lower transparency: market makers have informational advantages over other investors, reducing market transparency. Market makers'" (U.S.)
- HTML is simplified differently

**Liquidity row:**
- PDF has extensive content spanning two pages, including details about dark pools and iceberg orders not being officially available in mainland China, Block Trading Mechanism, Algorithms for splitting large trades
- HTML just says "Provided by all market participants directly" / "Primarily provided by designated market makers"

**Transaction Costs row:**
- PDF has detail about "Lower transaction costs: Buyer and seller quotes are matched based on specific rules, reducing costs beyond traditional market spreads" (China) and "Higher transaction costs: Increased trading costs are part of the profit earned by market makers" (U.S.)
- HTML says "Lower; simpler fee structure" / "More complex; maker/taker fees vary by venue"

**Action:** Replace all table cell content with the exact verbatim text from the PDF (pages 23-24). This is a significant content overhaul.

---

## Applicability of HFT Strategies in China Table — WRONG STRUCTURE AND CONTENT

The HTML table has 3 columns (Strategy, Applicable?, Key Constraints) but the PDF table has 4 columns (HFT Strategy, Strategy Description, Feasibility, Reason for Constraints). The HTML is missing the entire "Strategy Description" column and the constraint explanations are heavily summarized.

**PDF table structure (4 columns):**

| HFT Strategy | Strategy Description | Feasibility | Reason for Constraints |
|---|---|---|---|
| Market Making | Provides liquidity by simultaneously placing buy and sell orders to capture the bid-ask spread. | (constrained) | Auction trading system, T+1 rule, and restrictions on excessively frequent order placements and cancellations. |
| Liquidity Detection | Aims to detect and exploit hidden liquidity in the market, such as large orders in dark pools or iceberg orders. | Implementation of these HFT strategies is constrained in China's equity stock market | Dark pools and iceberg orders are not officially available in mainland China's centralized and transparent auction market. However, the strategy can still be adapted by analyzing visible order flows and market depth to detect potential large trades. |
| Cross-Exchange Arbitrage | Capitalizes on small price differences for the same asset across multiple exchanges. | (constrained) | Each stock is listed and traded on one exchange only. |
| Momentum Ignition | Attempts to trigger other traders to buy or sell by placing and canceling a series of orders to create artificial price momentum. | (constrained) | Excessively frequent order placement and cancellation are regulated and treated as abnormal trading practices in China. In the U.S., Momentum Ignition and Spoofing are also considered illegal, as they are considered to be market manipulation. |
| Quote Stuffing / Spoofing | Places a large number of orders quickly to create a false appearance of demand or supply, then cancels them. | (constrained) | (same as Momentum Ignition — shared cell in PDF) |
| Statistical Arbitrage (Stat Arb) | Uses statistical methods to identify pricing inefficiencies between correlated assets, typically involving mean reversion or co-integration strategies. | Not Constrained | (none) |
| Event Arbitrage | Responds to news events, earnings releases, or economic reports that cause temporary price movements. | (not constrained) | (none) |
| Order Flow Prediction | Analyzes patterns in order flow to predict short-term price movements. | (constrained) | Limited by speed constraints and regulatory oversight. |

**HTML table (current — wrong):**
- Missing the "Strategy Description" column entirely
- "Applicable?" column uses simplified labels (Limited, Partial, Not Feasible, Restricted, Prohibited, Applicable) instead of the PDF's more nuanced feasibility descriptions
- "Key Constraints" column has 1-line summaries instead of full PDF text
- Missing the shared feasibility cell that spans multiple rows in the PDF

**Action:** Add the "Strategy Description" column back. Replace all cell content with verbatim PDF text (pages 25-26). Update feasibility labels to match PDF.

---

## Trading Speed Improvements Table — WRONG STRUCTURE

The HTML table is laid out as rows-per-firm (firms in the left column), but the PDF table has firms as column headers across the top (firms go horizontally). The data values appear mostly the same, but the table orientation is completely different.

**PDF table structure:**
- **Orientation:** Firms are COLUMNS (horizontal), attributes are ROWS (vertical)
- **Column headers:** Organization | Jump Trading | Spread Networks | Arctic Fibre Inc. | Anova Financial Networks
- **Row headers:** Method, Cost, Time Saved, Improvement
- Spread Networks method says "Fiber optic cables crossing the Appalachian Mountains directly connecting to the New York Stock Exchange (NYSE)" — HTML drops "New York Stock Exchange" and just says "NYSE"
- Arctic Fibre improvement says "230 ms to 170 ms" — HTML says "230ms to 170ms" (minor spacing)

**HTML table (current — wrong orientation):**
- Firms are in the leftmost column (vertical), attributes are column headers
- This makes the table very wide and harder to read on narrow screens
- Should match PDF's orientation with firms as columns and attributes as rows

**Action:** Restructure the table so firms are column headers (horizontal) and Method/Cost/Time Saved/Improvement are row headers (vertical), matching the PDF layout. Verify "New York Stock Exchange (NYSE)" is spelled out fully for Spread Networks.

---

## HFT Comparison | U.S. and China Table — WRONG CONTENT

The HTML table has short 1-line summaries per cell. The PDF table (pages 27-28) has detailed multi-sentence explanations for each cell.

**Key differences by row:**

**Settlement System:**
- PDF U.S.: "T+0" + full paragraph about market-making strategies avoiding holding positions overnight, signals with overnight predictive capability, etc.
- PDF China: "T+1" + explanation about investors needing to hold a base stock position to execute intraday transactions
- HTML: Just "T+0" / "T+1" with no detail

**Short-Selling:**
- PDF U.S.: "Very few restrictions on short-selling through broker cooperation."
- PDF China: "Historically, HFT could use securities lending for short selling, but this practice was banned in 2024."
- HTML: "Well-developed; broad access to securities lending" / "Restricted; securities lending heavily regulated since 2024" — paraphrased, not verbatim

**Trading System:**
- PDF U.S.: "Primarily a market-maker system. High-frequency market-making strategies account for 60% of HFT strategies."
- PDF China: "Primarily an auction trading system. There are almost no high-frequency market-making strategies."
- HTML: "Market-maker based across 10+ exchanges, 50+ dark pools" / "Auction-based on 2 major exchanges (Shanghai, Shenzhen)" — different content

**Cross-Exchange Arbitrage:**
- PDF U.S.: "Cross-exchange arbitrage strategies are possible."
- PDF China: "Stocks can only be traded on one exchange, so cross-exchange arbitrage is not feasible."
- HTML: "Widely used; same stock tradable on multiple venues" / "Not feasible; each stock on one exchange only" — paraphrased

**Leverage:**
- PDF U.S.: "Leverage is virtually unrestricted. Some HFT strategies finance with leverage of more than ten times intraday."
- PDF China: "Leverage can be added through methods such as DMA. Historically, DMA could provide nearly 4 times leverage, but the 2024 guidelines limit DMA leverage to no more than 2 times."
- HTML: "Virtually unrestricted; 10x+ intraday common" / "DMA limited to 2x since April 2024" — heavily shortened

**Trade Speed Improvements:**
- PDF U.S.: "Major institutions are willing to invest tens of millions of dollars to shave off mere fractions of a millisecond in delays which has fueled an arms race for speed."
- PDF China: "China's market structure is relatively simple and most of the infrastructure is state provided, so improvement measures are less extreme. Therefore, the steps and costs involved in improving speed are far lower in China."
- HTML: "Multi-million dollar infrastructure arms race" / "Less extreme; state-provided infrastructure, few ms differences" — paraphrased

**HFT Volume Share:**
- HTML has "~50% of equity volume" / "~20% of equity volume" — need to verify these figures exist in the PDF table (they may come from the body text, not this specific table)

**Action:** Replace all cell content with verbatim PDF text from pages 27-28.

---

## Quants Outperformed Discretionary Offerings Chart — Replace with Screenshot

Same as the Barra Factor chart — this is too intricate to recreate (7 line series with weekly time-series data we don't have).

1. **Replace with a screenshot** from `assets/charts/` folder (need to identify which page has this chart — likely around page 29-30 of the PDF)
2. **Add a scroll-triggered animation:** As the user scrolls down, the chart image fades/slides into view. As they keep scrolling past it, it fades/slides out.
3. Remove the current Chart.js canvas for this chart entirely.

**Action:** Find the correct page screenshot, replace the chart with an `<img>` tag, and add Intersection Observer-based fade-in/fade-out scroll effect (same treatment as the Barra Factor chart).

---

## Quant MN & T0 Volatility/Sharpe Box Plots — Replace with Screenshot

Box plot charts with detailed statistical data we don't have. Same treatment as Barra Factor and Quants Outperformed charts.

1. **Replace with a screenshot** from `assets/charts/` folder (need to identify which page has this chart — likely around page 30-31 of the PDF)
2. **Add a scroll-triggered animation:** Fade-in on scroll down, fade-out as user scrolls past.
3. Remove the current Chart.js canvas for this chart entirely.

**Action:** Find the correct page screenshot, replace with `<img>`, add Intersection Observer fade-in/fade-out effect (same treatment as the other screenshot-replaced charts).

---

## EIF Annual Alpha Distribution Box Plots (2020–2023) — Replace with Screenshot

Three separate box plot panels (300 EIF, 500 EIF, 1000 EIF) with detailed statistical data we don't have. Same treatment as other screenshot-replaced charts.

1. **Replace with a screenshot** from `assets/charts/` folder (need to identify which page has this chart)
2. **Add a scroll-triggered animation:** Fade-in on scroll down, fade-out as user scrolls past.
3. Remove the current Chart.js canvas for this chart entirely.

**Action:** Find the correct page screenshot, replace with `<img>`, add Intersection Observer fade-in/fade-out effect.

---

## China's Top Quant Managers' Alpha During Feb 2024 Quant Quake — CHECK DATA ACCURACY

The HTML version looks great visually (user likes it). However, need to verify the data points are accurate against the PDF. If the line data can't be verified/matched exactly to the PDF, fall back to the screenshot solution:

1. **Replace with a screenshot** from `assets/charts/` folder
2. **Add scroll-triggered fade-in/fade-out animation**

**Preference:** Keep the current Chart.js version if data is accurate. Only replace with screenshot if data can't be verified.

**Note:** PDF title says "China's Top Quant Managers' Alpha Performance during Feb 2024 China Quant Quake" — HTML title drops "Performance" and "China" from the title. Minor difference.

---

## Onshore vs Offshore Access: Pros and Cons Table — WRONG CONTENT

The HTML table has short 1-line summaries. The PDF table has detailed multi-sentence explanations with bold lead-ins for each cell.

**Key differences by row:**

**Brokerage Fees:**
- PDF Onshore: "Lower fees: ~0.01%, significantly lower than offshore fees. Investors can save 2-4% in annual fees with high turnover rates around 100 times per year."
- PDF Offshore: "Higher fees: Approximately 0.02%-0.03%, making it more costly, especially for high-frequency strategies that are sensitive to transaction costs."
- HTML: "~0.01% — lower (1/5 to 1/3 of offshore)" / "~0.03–0.05% — higher" — note HTML says 0.03-0.05% but PDF says 0.02%-0.03%

**Latency:**
- PDF Onshore: "Lower latency: Faster execution with lower latency, suitable for high-frequency and ultra-high-frequency trading."
- PDF Offshore: "Higher latency: Generally, 10-100 ms slower than onshore, affecting high-frequency strategies due to alpha erosion; recent and potential regulatory measures targeting HFT may reduce this impact."
- HTML: "Lower — direct exchange access" / "Tens to ~100ms higher than onshore" — heavily shortened

**Trading Days:**
- PDF Onshore: "More trading days: Not affected by holidays and weather related closures in Hong Kong, offering more trading days annually."
- PDF Offshore: "Fewer trading days: Stock Connect trading is subject to both Hong Kong and mainland China holidays and weather related closures in Hong Kong, resulting in around 8 fewer trading days yearly. The government is working on this issue. Trading through QFII with a PB is another solution, though it is generally more expensive."
- HTML: "More days — mainland holidays only" / "~8–20 fewer days (HK + mainland holidays)" — note HTML says "8-20" but PDF says "around 8"

**Leverage & Securities Lending:**
- PDF Onshore: "Restricted: Limited options for leverage and securities lending onshore, limiting certain strategy flexibility."
- PDF Offshore: "More accessible: Easier to use leverage and access securities lending, favoring leveraged market-neutral and short-focused quant strategies."
- HTML: "Restricted — DMA max 2x; limited securities lending" / "More accessible — flexible leverage and short selling" — paraphrased

**FX Impact:**
- PDF Onshore: "Simpler FX impact: Only impacted during subscription and redemption periods, allowing investors to choose currency conversion timing."
- PDF Offshore: "More complicated FX impact: Real-time FX fluctuations affect offshore investors due to foreign exchange settlements when realizing profits with investment in RMB assets."
- HTML: "Only at subscription/redemption; timing control" / "Real-time FX fluctuations during transactions" — shortened

**Capital Inflow Requirement:**
- PDF Onshore: "Funds must enter mainland China: Weather through a QFII license or a broker's QFII/RQFII channels via swap structure, this approach essentially involves transferring funds into China."
- PDF Offshore: "No direct inflow required: Offshore access does not require direct fund inflows into mainland China, providing greater flexibility for capital management."
- HTML: "Funds must enter mainland China (QFII or broker swap)" / "Funds remain offshore" — shortened, and PDF row is called "Capital Inflow Requirement" not just "Capital Inflow"

**Action:** Replace all cell content with verbatim PDF text. Fix the offshore brokerage fee range (0.02%-0.03%, not 0.03-0.05%). Fix trading days (around 8, not 8-20).

---

## AI's Role In An Investment Process Chart — X-Axis Labels Messy

Data is correct. The x-axis labels need cleanup — currently only showing abbreviated/partial labels. Per the PDF, the full x-axis labels should be:
1. Identify patterns and trends in market behaviour
2. Optimize portfolio allocation and risk management
3. Develop and test investment strategies
4. Monitor and adjust investment positions in real-time
5. Perform sentiment analysis on news, earnings calls and social media
6. Automate timing of trading decisions

**Action:** Fix x-axis labels to show the full text from the PDF, properly wrapped/rotated so they're readable.

---

## China Market Index Definition and Comparison — Style Mismatch

The HTML version uses a custom horizontal bar-style layout (stacked rows with colored bars). The PDF is a proper table with columns: Market Cap | Index | Stocks Included (Ranked by Market Value) — with a visual bar spanning across to show the range, plus a "Top X" column on the right.

**Key differences:**
- PDF has a clear table structure with columns and a visual bar overlay showing the stock ranges
- HTML uses full-width colored rows that look like a different component entirely
- PDF labels say "Top 1-300", "Top 301-800", "Top 1001-1800", "Top 1801-3800" in the rightmost column — HTML says "Stocks 1–300", "Stocks 301–800", "Stocks 801–1800", "Stocks 1801–3800"
- Note: PDF says CSI 1000 = "Top 1001-1800" but HTML says "Stocks 801-1800" — the stock range numbers differ for CSI 1000

**Action:** Double-check whether these can be made more similar to the PDF's table-with-visual-bar style. Also verify the correct stock ranges (especially CSI 1000: is it 801-1800 or 1001-1800?).

---

Things to check for in each chart/table:
- 