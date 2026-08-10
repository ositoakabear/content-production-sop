# Kickstarter Product Post SOP

This SOP turns a Kickstarter or similar product lead into a WeChat-ready product observation article, with optional Xiaohongshu adaptation and WeChat draft publishing.

Before drafting, read `../../docs/editorial/wechat-general-writing-skill.md`. Its approved author-voice baseline is mandatory; this playbook adds Kickstarter-specific research, structure, risk, and packaging rules without replacing that voice.

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
- Follow the canonical source priority in `../../docs/assets/image-asset-workflow.md`: first-party official originals first, credible public or media originals second, and generated visuals only when real imagery is unavailable or the visual is explicitly conceptual.
- Generated visuals are acceptable for scenario composites, competitor-type diagrams, or clearly labeled illustrations, but not as substitutes for available real products, people, logos, UI, events, or documents.
- Founder/team sections should use real founder or team images when available.
- Store final assets in the product folder, not in temporary output folders.
- Use numbered semantic filenames: `01_<product>_title_cover.jpg`, `02_<product>_lifestyle.jpg`, `03_<product>_install_detail.jpg`, `04_<product>_founders.jpg`, `05_<product>_scenario_grid.jpg`, `06_<product>_competitors.jpg`, `07_<product>_transition.gif`.
- Lock title-cover copy to two text levels: `本周好物观察` and the official product name. Do not add a slogan, core selling point, feature phrase, emotional hook, campaign result, or duplicate article headline.

See `../../docs/assets/image-asset-workflow.md` for shared image-package conventions.

## 4. WeChat Article Structure

Recommended structure:

1. Universal "势差" opening banner.
2. Opening scene: start from a real user pain point or surprising product contrast.
3. One-sentence value judgment.
4. `PART 01`: founder, creator, brand story, and campaign credibility.
5. `PART 02`: project overview with campaign timing, funding result, price, delivery, and core functions.
6. `PART 03`: real pain point or creative origin, framed as "it truly solves..."
7. `PART 04`: function and experience, organized around concrete usage scenarios.
8. `PART 05`: competitor comparison as vertical cards, not a wide table.
9. `PART 06`: risks, target audience, and market judgment.
10. `REVIEW`: personal observer commentary.
11. Platform-native official-account profile card, following the shared ending-order rule.
12. `LINKS`: source navigation and crowdfunding risk reminder.

## 5. Writing Rules

- Do not add a duplicate in-article title card by default. When a project intentionally keeps an H1, the external title and in-article H1 should not be identical.
- Start with a concrete friction chain: what the user wants to do, what stops them, and what workaround they currently tolerate.
- Explain product value with sentences like "it sells not A, but B" only when the contrast is genuinely useful.
- Follow the shared emphasis system: render underlined prices, parameters, dates, mechanisms, or selected key phrases as black text with `border-bottom:2px dashed #3aaa35;padding-bottom:1px;`. Do not use a native solid underline.
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
