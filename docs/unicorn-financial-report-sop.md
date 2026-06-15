# Weekly Unicorn Financial Report SOP

This SOP turns a unicorn company research topic into a WeChat-ready long-form analysis article, with optional Xiaohongshu adaptation and supporting visuals.

## 1. Positioning

The article should read like a concise business case study, not a raw data dump.

Target reader:

- Interested in startups, venture capital, emerging markets, and business models
- Reads on mobile
- Wants clear judgment, not only facts

Preferred tone:

- Clear, compact, analytical
- Public-account friendly
- Avoid over-academic structure
- Use short paragraphs, strong section titles, and visual summary blocks

## 2. Topic Selection

Pick a company that meets at least two of the following:

- Recently disclosed important financial or operational data
- Has a clear business model shift, profitability milestone, or funding event
- Represents a broader sector trend
- Has enough public information to support founder, investor, competitor, and business model analysis
- Is not repetitive with recent articles

For each candidate, record:

- Company name
- Country and sector
- Latest valuation or funding round
- Why it matters now
- Core question the article should answer

Example core question:

> Has Kavak proved that a heavy-asset used-car ecommerce model can work profitably in Latin America?

## 3. Source Verification and Claim Hygiene

For private companies, do not treat user-provided financial claims as automatically audited facts.

Classify each important claim before drafting:

- `Verified`: supported by company filings, press releases, investor materials, credible media interviews, or official transaction announcements
- `Management stated`: directly attributed to executives or company representatives, but not independently audited in public
- `Reported`: published by credible media or transaction advisers, but not visible in primary filings
- `Inferred`: analyst interpretation or model-based conclusion
- `Unverified`: should be removed, softened, or explicitly caveated

Private-company rule:

- If a full audited financial statement is not public, avoid saying the article is based on a complete audited annual report.
- Replace unsupported precision with source-aware wording such as "management said," "public reporting indicates," "the company appears to be," or "the strategic signal is."
- Keep valuation dates clear. If the latest public valuation comes from an older funding round, say so.
- Separate EBITDA, adjusted EBITDA, free cash flow, revenue, gross profit, and net profit. Do not collapse them into one profitability claim.
- Preserve uncertainty in risk sections instead of forcing a banker-style certainty.

Minimum source log:

- Founder or company profile source
- Latest valuation or financing source
- Profitability or operating milestone source
- Strategic investor or acquisition source
- Fintech, regulatory, or asset sale source when relevant
- Any article or public account used only as style reference, not factual source

## 4. Research Inputs

Collect information in six buckets.

### Founder Team

Include both the founding trigger and the team's background.

Minimum details:

- Founder names and roles
- Prior operating, platform, consulting, finance, or technology experience
- Why their background fits the market problem
- The personal or market pain point that led to the company

### Financial and Operational Data

Prioritize the latest data points:

- Transaction volume
- Revenue or gross profit drivers
- Profitability milestone
- Financing or securitization scale
- User penetration or attach rate
- Market geography and expansion/contraction

Connect each data point to a business implication:

- What changed?
- Why does it matter?
- What should readers watch next?

### Revenue Pillars

Break the model into clear layers:

- Core revenue source
- Profit driver
- Recurring or high-margin add-ons

For marketplace or commerce companies, separate:

- Transaction gross margin
- Financing or fintech revenue
- SaaS, service, subscription, warranty, or advertising revenue

For super-app or delivery companies, also separate:

- Marketplace commissions and user fees
- Subscription membership
- Retail media or merchant advertising
- Fintech or credit products
- Fulfillment density and unit-cost advantages

### AI and Technology

Do not mention AI only as a label. Explain where it changes unit economics.

Useful analysis dimensions:

- Pricing
- Inventory allocation
- Demand prediction
- Workflow automation
- Credit risk assessment
- Customer conversion
- Fraud detection

Tie AI usage to business outcomes:

- Lower acquisition cost
- Faster inventory turnover
- Better gross margin
- Lower default rate
- Higher conversion
- Better supply quality

If AI is not central to the company, replace this section with the relevant operating system, such as logistics density, payments infrastructure, supply standardization, or regulatory arbitrage.

### Competitors

Choose two to four competitor types rather than only named companies.

Compare on:

- Asset model: self-operated, marketplace, hybrid
- Supply sourcing or fulfillment model
- Trust or quality-control layer
- Financing or payments control
- Technology depth and data advantage
- Geographic focus and localization

### Investors

Introduce major investors with enough background to explain why they matter.

For each key investor:

- Institution name
- Founding or reputation background
- Investment style
- Why the company fits its thesis
- What the investor likely expects next
- Whether the investor is purely financial or strategically relevant

## 5. Article Structure

Recommended WeChat structure:

1. Opening judgment card
2. Founder team
3. Core financial and operational data
4. Revenue pillars
5. AI, technology, or operating system
6. Competitor comparison
7. Strategic conclusion
8. Key investor background and investment logic
9. Personal commentary section
10. Final summary

Recommended recurring commentary block:

> Weekly Unicorn Observer Axiong Commentary

This block should provide a clear personal judgment, not repeat the article.

## 6. WeChat HTML Packaging

Mobile reading comes first. Build the HTML as a paste-ready WeChat package, not as a general web page.

Use:

- Inline styles, because external CSS and class names are unreliable in WeChat
- Short paragraphs, usually two to four lines on mobile
- Numbered section titles
- Light background cards for key data
- Highlight boxes for personal judgment
- Image captions under each visual
- Relative image paths, such as `images/business-network.png`, before the upload script converts images to WeChat CDN URLs

Avoid:

- Long unbroken paragraphs
- Dense tables
- `<ul>` and `<li>` lists when custom bullet paragraphs are safer
- Horizontal scrolling tables for competitor comparisons
- External image links in the final draft
- In-image AI-generated text when the text needs to be accurate

Suggested local package convention:

```text
E:\public-account\unicorn\<Company>\
  <company>-wechat.html
  images\
    title-master.png
    title-cover-2.35x1.jpg
    title-cover-1x1.jpg
    founder-team-source-card.jpg
    business-network.png
    revenue-or-monetization.png
    competitor-comparison.png
    raw-generated\
```

Validation:

- Confirm every `<img src="...">` points to an existing local file.
- Check that no image file is only left in a temporary generated-image folder.
- If browser security policy blocks local preview from a non-workspace drive, do a static resource check and manually preview through the WeChat editor or a permitted local path.

## 7. Visual Asset Workflow

For a full article package, prepare:

- Title cover safe master
- 2.35:1 safe-crop cover
- 1:1 safe-crop cover
- Founder or management team image from a public source when available
- Business or revenue-pillar infographic
- Key-event visual, such as a three-panel turning-point image
- AI, operating system, or monetization visual
- Competitor comparison infographic optimized for mobile

Important:

- Do not generate fake founder group photos.
- If a real group photo is unavailable, download public founder headshots and build a clearly labeled source card.
- If using a public media photo, keep source attribution in the caption or source notes.
- For generated images, avoid real logos and exact trademarks unless the rights and source are clear.
- Keep essential title-cover content inside a central square safe area so it survives both wide and square crops.
- Use generated visuals for concepts, systems, and symbolic model comparisons; use real images for real people.
- Prefer object-based infographics without embedded text. Put labels and explanation in the article caption where they are editable and accurate.
- For mobile infographics, avoid small table text. Use stacked cards or large symbolic panels.

## 8. Review Checklist

Before publishing:

- Does the opening state the core judgment quickly?
- Are unsupported private-company claims softened or removed?
- Is founder background more than just founding origin?
- Are core data points tied to business model implications?
- Is AI or technology explained through concrete operating use cases?
- Does competitor comparison explain why the model is different?
- Does investor background lead to a complete investment logic?
- Does the final commentary add a personal view?
- Are all visuals readable on a phone?
- Are generated images free of fake logos, fake people, and garbled text?
- Are public image sources credited when needed?
- Does the local output package contain the HTML, final images, and raw generated-image backups?
- Has the WeChat draft been saved and checked after editing?
