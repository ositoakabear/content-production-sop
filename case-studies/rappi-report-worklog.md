# Case Study: Rappi Unicorn Financial Report

This document records the production workflow for the Rappi weekly unicorn financial report and the iteration it added to the SOP.

## 1. Initial Topic

Company:

- Rappi
- Colombia / Latin America
- On-demand delivery, instant retail, super-app, fintech, and merchant advertising

Initial angle:

> Latin America's delivery super-app is moving from capital-burning growth to positive adjusted EBITDA, strategic partnership optionality, and IPO readiness.

Core thesis:

> Rappi is not only a food-delivery app. It uses high-frequency local delivery as the entry point, instant retail and merchant ads as margin expansion layers, and fintech partnerships as a way to monetize the ecosystem without carrying all balance-sheet risk itself.

## 2. Reference Inputs

The user provided a detailed draft with strong claims about FY2025 financials, Amazon investment, Banorte's acquisition of the RappiCard Mexican entity, valuation, and potential IPO timing.

A reference WeChat article was also provided:

- `https://mp.weixin.qq.com/s/2bZ9kKXMya1COPtMm9Cm3A`

That reference was treated as a layout and series-style reference, not as a factual source for Rappi.

## 3. Fact-Checking Iteration

The first important workflow decision was to avoid treating all provided figures as audited public facts.

What was verified or supported by public sources:

- Rappi's last widely reported private valuation of about $5.25 billion came from its 2021 Series F round.
- CEO Simon Borrero publicly discussed positive EBITDA momentum and potential IPO-window evaluation in 2026.
- Amazon reportedly invested $25 million through a convertible instrument with warrants tied to future ownership potential.
- Banorte announced the acquisition of the remaining ownership in Tarjetas del Futuro, the RappiCard Mexico operating entity, and a long-term commercial agreement.
- The three co-founders and YC W16 background were supported by the Y Combinator company profile.

What was softened:

- Exact FY2025 consolidated revenue, dark-store counts, loan balances, and audited-report language were not presented as audited public disclosures.
- The article avoided saying Rappi had published a complete public FY2025 audited financial statement.
- EBITDA, adjusted EBITDA, free cash flow, and net profit were kept distinct.

Editorial lesson:

> For private unicorn financial reports, confidence grading is part of the writing workflow. If a number cannot be traced to a public primary or credible secondary source, the article should either caveat it, soften it, or remove it.

## 4. Article Draft Iteration

The first article version followed the existing unicorn SOP structure:

1. Opening judgment
2. Company identity
3. 2025 strategic signals
4. Revenue pillars
5. Founder team
6. Competitive moat
7. Risks
8. Weekly observer commentary
9. Final summary

The strongest framing became:

> Rappi has compressed the super-app story into three things capital markets can understand: profitability, cash flow discipline, and strategic buyer optionality.

This was more useful than a broad company profile because it connected the company to a timely capital-market question.

## 5. WeChat HTML Iteration

The user asked for HTML based on the reference public-account article.

The reference style was translated into a reusable HTML pattern:

- Green numbered section markers
- Light green information cards
- Orange judgment/commentary boxes
- Short mobile-first paragraphs
- Vertical competitor cards instead of dense tables
- Inline styles instead of external CSS
- No `<ul>` / `<li>` dependency for key bullet sections

Local first output:

- `C:\Users\12986\Documents\Creation\rappi-wechat.html`

Final packaged output after the user requested a dedicated folder:

- `E:\public-account\unicorn\Rappi\rappi-wechat.html`

Editorial lesson:

> The WeChat HTML deliverable should be packaged with its images from the start. A standalone HTML file is useful for drafting, but the publishing unit is the folder containing HTML plus final image assets.

## 6. Visual Asset Production

The user requested six visual assets:

1. Generated title image that works in both 2.35:1 and 1:1 crops
2. Founder-team image, preferably downloaded
3. Generated Rappi business network image
4. Generated 2025 three-mainline image
5. Generated or downloaded commercialization visual
6. Generated comparison image against Mercado Libre, iFood, Uber Eats, and DoorDash

Final local asset folder:

```text
E:\public-account\unicorn\Rappi\images\
```

Final selected assets:

- `title-master.png`
- `title-cover-2.35x1.jpg`
- `title-cover-1x1.jpg`
- `founder-team-yc-card.jpg`
- `business-network.png`
- `three-mainlines-2025.png`
- `monetization-funnel.png`
- `competitor-comparison.png`

Raw generated backups:

```text
E:\public-account\unicorn\Rappi\images\raw-generated\
```

A rejected generated business-network image was kept in raw backups because the central mark looked too close to Rappi's official moustache-like logo.

Visual lesson:

> Generated conceptual images should avoid real logos, fake brand marks, and embedded text. For accurate labels, keep the text in captions or HTML. For real people, use downloaded public-source images instead of generated portraits.

## 7. Founder Image Iteration

A real founder group photo was not downloaded. Instead, public YC founder avatars were downloaded from the Rappi company profile:

- Simon Borrero
- Sebastian Mejia
- Felipe Villamarin

These were converted into a single source-labeled founder card:

- `founder-team-yc-card.jpg`

A first generated card used accented characters and Chinese text, but the image-rendering pipeline garbled some characters. The card was regenerated with ASCII text only:

- `Rappi Founding Team`
- `YC W16 public founder avatars`
- `Source: Y Combinator company profile / public founder avatars`

Visual lesson:

> If an image contains text, prefer ASCII or use HTML captions. AI-generated or programmatically rendered multilingual text should be checked visually before delivery.

## 8. HTML Asset Insertion

The final HTML references images with relative paths:

```html
<img src="images/title-cover-2.35x1.jpg" ...>
<img src="images/business-network.png" ...>
<img src="images/three-mainlines-2025.png" ...>
<img src="images/monetization-funnel.png" ...>
<img src="images/founder-team-yc-card.jpg" ...>
<img src="images/competitor-comparison.png" ...>
```

Each image has a caption explaining the intended reading, so the graphic can stay mostly text-free.

The in-app browser blocked direct preview of the `E:` drive file URL for security-policy reasons. Instead of trying to bypass that policy, a static resource validation was run:

- Confirmed all six referenced images existed
- Confirmed there were no missing image paths
- Listed dimensions and file sizes for all final image assets

Validation lesson:

> If local preview is blocked by browser policy, do not bypass it. Do static file validation and preview through a permitted surface, such as the WeChat editor or a copied workspace path.

## 9. SOP Changes Triggered by This Case

This Rappi workflow added or strengthened these SOP rules:

- Add a private-company source verification and claim-confidence step.
- Treat reference WeChat articles as layout references, not factual sources.
- Package final deliverables into a stable local folder: HTML plus images.
- Keep title-cover content inside a central square safe area before exporting 2.35:1 and 1:1 crops.
- Prioritize real public-source images for founders and management teams.
- Use generated images for systems, business models, and symbolic comparisons.
- Avoid logos, fake people, and embedded text in generated graphics.
- Keep raw generated images for rollback and auditability.
- Validate local image paths before handing off the HTML.

## 10. Reusable Takeaways

- Start with a sharp capital-market question, not a company description.
- Source-grade private-company data before drafting.
- Make the article's thesis survive the removal of unsupported figures.
- Use public-source portraits for real people and generated visuals for abstract business systems.
- Design title images as a safe master first, then crop.
- Keep captions in HTML so image text does not become a publishing risk.
- Deliver the article as a complete local package, not only as pasted text.
