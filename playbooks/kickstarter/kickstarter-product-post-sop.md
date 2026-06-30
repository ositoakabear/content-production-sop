# Kickstarter Product Post SOP

This SOP turns a Kickstarter or similar product lead into a WeChat-ready product observation article, with optional Xiaohongshu adaptation and WeChat draft publishing.

## 1. Positioning

The article should read like a product and market observation, not a feature list.

Target reader:

- Interested in new consumer products, hardware, DTC brands, crowdfunding, and practical product design
- Reads on mobile
- Wants to understand why a product exists, who it is for, what risk remains, and what it says about a larger consumption shift

Preferred tone:

- Specific, concrete, and lightly personal
- Product-first, but not purely promotional
- Clear about campaign uncertainty and product limitations
- Judgment-led: explain what the product really sells, not only what it does

## 2. Workflow

1. Collect product material, campaign page, official site, press coverage, creator story, images, GIFs, and campaign trackers.
2. Create a product-local asset folder, such as `.../Kickstarter/<ProductName>/`.
3. Download or generate final images into that folder with numbered semantic names.
4. Draft the WeChat article using the structure below.
5. Adapt the same facts into a Xiaohongshu post if needed.
6. Package the WeChat HTML with inline styles and local image references.
7. Run the WeChat publishing script or create a rich-copy HTML page.
8. Preview on mobile and fix image order, captions, cards, links, and risky formatting.

## 3. Material And Asset Rules

- Product images must show the real product whenever possible.
- Use official or credible media images before generated images.
- Generated visuals are acceptable for scenario composites, competitor-type diagrams, or clearly labeled illustrations.
- Founder/team sections should use real founder or team images when available.
- Store final assets in the product folder, not in temporary output folders.
- Use numbered semantic filenames: `01_<product>_title_cover.jpg`, `02_<product>_lifestyle.jpg`, `03_<product>_install_detail.jpg`, `04_<product>_founders.jpg`, `05_<product>_scenario_grid.jpg`, `06_<product>_competitors.jpg`, `07_<product>_transition.gif`.

See `../../docs/assets/image-asset-workflow.md` for shared image-package conventions.

## 4. WeChat Article Structure

Recommended structure:

1. Universal "势差" opening banner.
2. Title card with the article-specific H1.
3. Opening scene: start from a real user pain point or surprising product contrast.
4. One-sentence value judgment.
5. `PART 01`: founder, creator, brand story, and campaign credibility.
6. `PART 02`: project overview with campaign timing, funding result, price, delivery, and core functions.
7. `PART 03`: real pain point or creative origin, framed as "it truly solves..."
8. `PART 04`: function and experience, organized around concrete usage scenarios.
9. `PART 05`: competitor comparison as vertical cards, not a wide table.
10. `PART 06`: risks, target audience, and market judgment.
11. `REVIEW`: personal observer commentary.
12. `LINKS`: source navigation and crowdfunding risk reminder.

## 5. Writing Rules

- External title and in-article H1 should not be identical.
- Start with a concrete friction chain: what the user wants to do, what stops them, and what workaround they currently tolerate.
- Explain product value with sentences like "it sells not A, but B" only when the contrast is genuinely useful.
- Do not make the product win every comparison. A credible product post should name the short board.
- Risks must be product-specific: delivery, compatibility, app dependency, battery life, consumables, repair, setup, children/pets, outdoor/weather, or after-sales.
- If a product has DTC, retail, Shark Tank, prior Kickstarter, fulfillment, press, or creator signals, add a business-model or go-to-market paragraph.

## 6. Competitor Comparison

Use vertical dimension cards because WeChat mobile strips or breaks many wide-table layouts.

Good comparison dimensions:

- Installation/setup
- Power or maintenance
- Brightness/performance
- Portability
- Decoration or product feel
- Price and value
- Campaign credibility

Keep the competitor set stable across dimensions. For example, compare the product to hardwired alternatives, plug-in alternatives, cheap utility alternatives, and smart/portable alternatives.

## 7. Xiaohongshu Adaptation

The Xiaohongshu version should preserve facts but change the reading rhythm:

- More first-person and mobile-native
- Shorter paragraphs
- Light emoji
- Image placeholders such as `(配图 1: 实物挂墙图)`
- Tags for product category, audience, scenario, and fixed series label

See `../../docs/platforms/xiaohongshu-adaptation.md`.

## 8. Packaging And Publishing

- Use inline HTML styles for WeChat.
- Avoid `<ul>/<li>`, `display:flex`, and horizontal scrolling comparison tables.
- Use local image paths before the publish script uploads and replaces image URLs.
- Keep the clean article HTML separate from the rich-copy HTML with copy buttons.
- Use `scripts/wechat/publish_wechat.py` or the skill-local script for draft add/update.

See `../../docs/platforms/wechat-rendering-and-api-pitfalls.md`.
