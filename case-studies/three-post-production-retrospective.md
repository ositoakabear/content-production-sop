# Case Study: Three Unicorn WeChat Posts Production Retrospective

This document summarizes the production lessons from the first three weekly unicorn public-account articles:

1. Kavak: first full production run
2. Rappi: second article and packaging iteration
3. Uala: third article and voice/visual calibration iteration

The purpose is to convert the accumulated experience into reusable rules for future `每周独角兽观察` articles.

## 1. Three-Article Progression

### Kavak: First Full Run

Published title:

> Kavak：拉美二手车独角兽的盈利拐点

Kavak established the base structure for a unicorn financial-analysis article:

- Opening judgment
- Founder team
- Financial and operating data
- Revenue pillars
- AI or operating system
- Competitor comparison
- Strategic risk section
- Investor background and investment logic
- Personal commentary

Core production lesson:

> The article should not read like a company encyclopedia. It should answer one business question. For Kavak, the question was whether a heavy-asset used-car ecommerce model could reach a profitability inflection point in Latin America.

### Rappi: Second Article and Packaging Iteration

Published title:

> 拉美版美团不烧钱了：Rappi的52.5亿美元IPO赌局

Rappi added a stronger publishing workflow:

- Private-company claim grading
- Explicit source notes
- WeChat HTML package with relative image paths
- Rich-copy HTML for pasting into the WeChat editor
- Dedicated `images/` folder
- `raw-generated/` backups
- Founder-card production from public-source avatars
- Caption-first visual explanation to avoid in-image text risk

Core production lesson:

> The publishing unit is not only the article text. It is the full production package: draft HTML, rich-copy HTML, final images, source/rejected assets, raw generated backups, and the final saved WeChat archive.

### Uala: Third Article and Calibration Iteration

Published title:

> 拉美数字银行Uala：腾讯押注的下一个Nubank？

Uala strengthened the series voice and company-specific visual logic:

- Final-draft voice calibration
- Name-origin handling for unfamiliar companies
- Investor logic near the financing hook
- Investor categories explained in plain language
- China-relevant comparison without unsupported technology-transfer claims
- Opening brand-identity image built from official product assets
- Rejected visual direction preserved in `rejected-rappi-like/`
- Typography adjusted for long mobile financial reading

Core production lesson:

> Prior articles can guide asset quantity and workflow, but they should not become a visual-style template. Each unicorn needs visuals that reflect its actual product surface and business model.

## 2. Reusable Content Lessons

### Start With A Capital-Market Question

Each article should be framed by a question that matters now:

- Kavak: Can a heavy-asset used-car model become profitable in Latin America?
- Rappi: Can a formerly capital-burning super-app become IPO-ready?
- Uala: Can a wallet/card fintech become a licensed digital-bank balance-sheet story?

The opening should quickly say:

- What the company is
- What it is not merely
- Why this moment matters
- What question the article will answer

### Write From Model Difference, Not Company Description

Avoid listing facts in company-profile order. Each section should advance the business model logic:

- Kavak is not only a used-car ecommerce company; it is vehicle trust infrastructure plus auto finance.
- Rappi is not only food delivery; it is a high-frequency local-services entry point with advertising, membership, retail, and fintech layers.
- Uala is not only a wallet; it is trying to turn account relationships into deposits, credit, merchant acquiring, insurance, and wealth products.

### Let Section Order Follow Reader Curiosity

Do not force a fixed module sequence.

- Kavak can start with founder-market fit because the heavy operating model depends on the team.
- Rappi should move quickly into 2025 profitability, Amazon, and Banorte because those are the event hooks.
- Uala should place investor logic near the financing event because Tencent, Allianz X, and Nubank comparisons are part of the reader hook.

### Treat Investors As Thesis Carriers

Investor sections should answer what each kind of capital is buying:

- a16z: software and finance rebuilding a traditional heavy-asset industry
- Amazon: optionality around local instant fulfillment infrastructure
- Banorte: regulated financial operation and partnership economics
- Allianz X: digital insurance distribution inside banking scenarios
- Tencent / D1: mobile finance, growth equity, and public-market asset potential
- SoftBank / Soros: Latin American financial inclusion and macro-sensitive long-cycle repricing

### Compare Models, Not Only Competitors

Use model categories:

- Kavak: self-operated platform, traditional dealers, marketplace platforms, mature-market online used-car models
- Rappi: super-app, ecommerce marketplace, local food-delivery leader, global delivery platforms
- Uala: licensed digital bank, listed neobank, marketplace wallet, credit-card fintech, traditional bank

This makes the comparison more durable than a list of brand names.

## 3. Source and Claim Lessons

Private-company articles need a mandatory `资料口径` block when they discuss valuation, IPO timing, profitability, financing, or investor logic.

Useful closing pattern:

- State the main source categories.
- Separate official announcements from media reports and management comments.
- Say when complete audited financial statements are not publicly available.
- Clarify that financial and valuation judgments are based on public disclosures, company statements, credible reports, and user-provided material.
- Add that the article is not investment advice.

Rappi and Uala made this rule clearer than Kavak. Future articles should treat the source-notes block as a standard deliverable, not an optional appendix.

## 4. Title Lessons

Working titles and final published titles may differ.

Examples:

- Rappi working direction: analytical IPO/profitability framing
- Rappi final title: `拉美版美团不烧钱了：Rappi的52.5亿美元IPO赌局`
- Uala working direction: `腾讯押注的Uala，凭什么在拉美值32亿美元？`
- Uala final title: `拉美数字银行Uala：腾讯押注的下一个Nubank？`

Reusable rule:

> Title calibration is a separate publishing step. The final title should be sharper for WeChat readers while preserving the real thesis and source support.

Good public-account title hooks include:

- Familiar Chinese analogy, such as Meituan, Tencent, WeBank, or Nubank
- Concrete valuation or financing number
- IPO or profitability question
- A turning point, such as no longer burning cash, moving into banking, or reaching profitability

## 5. Visual and Asset Lessons

### Keep Working Assets Separate From Published Archives

The final WeChat-saved page creates a large `<Final Published Title>.html` and `<Final Published Title>_files/` folder. These are useful as a published archive, but they contain platform CSS, scripts, CDN artifacts, and opaque filenames.

The editable production package should remain:

```text
<company>-wechat.html
<company>-wechat-rich-copy.html
images/
  source/
  raw-generated/
  rejected-<reason>/
```

### Count Cover Images Separately From Body Images

Draft HTML image references do not always match final published body image counts. Some title images may become cover/share assets rather than body images.

Therefore, validate separately:

- Cover/share images
- Body images
- Founder or brand-identity images
- Generated conceptual images
- Source assets
- Raw and rejected assets

### Preserve Source and Rejected Folders

`images/source/` should store official product, brand, or public-source assets used to build identity images.

`rejected-<reason>/` should store rejected directions only when they teach a reusable lesson. Uala's `rejected-rappi-like/` folder is a good example: it preserves the reason that a visual direction was rejected, not just the discarded files.

### Use Real Assets For Identity And People

- Use official or public-source brand/product images for the opening identity image.
- Use real public founder photos or source-labeled public avatars for founders.
- Use generated images for abstract systems, model comparisons, business networks, and symbolic monetization flows.
- Avoid fake logos, fake people, and embedded multilingual text.
- Keep explanatory text in captions when accuracy matters.

## 6. Series Naming Standard

Use these labels consistently:

- Series name: `每周独角兽观察`
- Personal commentary block: `每周独角兽观察员点评`

Avoid near-duplicates unless intentionally testing a new column format:

- `每周独角兽财报观察`
- `每周独角兽财报研读`
- `每周独角兽观察员阿熊点评`
- `观察员阿熊`

The stable naming helps future articles feel like one series instead of isolated posts.

## 7. Updates Added To The Main SOP

This three-article review triggered these SOP updates:

- Add title calibration as a required publishing step.
- Add post-publish recovery review after saving the final WeChat page.
- Add `*-wechat-rich-copy.html` to the standard deliverable package.
- Separate cover/share image validation from body image validation.
- Add `images/source/` and `rejected-<reason>/` to the local asset convention.
- Make `资料口径` mandatory for private-company articles with material financial or valuation claims.
- Standardize series naming as `每周独角兽观察` and `每周独角兽观察员点评`.
