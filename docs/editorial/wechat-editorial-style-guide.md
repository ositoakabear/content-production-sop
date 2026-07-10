# WeChat Editorial Style Guide for 势差

This guide applies to paste-ready WeChat articles published under the public account "势差".

## 1. Brand Positioning

"势差" should feel like a calm editorial notebook for products, brands, new consumption, startups, AI, and cross-border business. The visual language should be analytical, restrained, and slightly sharp: warm paper background, black structural shapes, and one small red accent.

Avoid a marketing-poster look. Do not use loud gradients, busy decorative graphics, or stock-style atmosphere images when the article is an analysis or product observation.

## 2. Opening Banner

Use a branded opening banner before the article title block when the article is packaged as a finished WeChat post.

Default universal banner asset:

```text
/Users/axiong/Desktop/文档集合/公众号/头像/shicha_editorial_banner.gif
```

Current product-local copy:

```text
/Users/axiong/Desktop/文档集合/公众号/Kickstarter/Poplight/00_shicha_editorial_banner.gif
```

Recommended banner specs:

- Size: `1080 x 300`
- Format: GIF preferred; static PNG is acceptable when GIF upload or preview fails
- Visual basis: use the "势差" avatar language, with off-white paper, black rising geometric planes, and a small red differential mark
- Content language: keep only the logo, `势差`, and one cross-column slogan
- Default slogan: `看见新商业背后的结构势能`
- Placement: first visual inside the article body, before the title card
- Styling in HTML:

```html
<section style="margin:0 0 22px;text-align:center;">
  <img src="..." alt="势差公众号通用动图 banner" style="display:block;width:100%;height:auto;" />
</section>
```

## 3. Mini-Program Entry

Do not add a mini-program entry until the account has a confirmed mini-program appid, landing path, and entry image.

When available, add a picture-style mini-program entry after the opening banner or in the bottom conversion area. Use the WeChat image mini-program format rather than a plain text link.

Required fields to collect before implementation:

- Mini-program appid
- Landing path
- Display nickname
- Entry image
- Whether the entry is for a product, report, resource pack, or account service

## 4. Body Typography

For mature WeChat editorial packaging, default to a denser media-style reading rhythm:

- Body font size: `17px`
- Body line-height: `1.75em`
- Body letter-spacing: `0.034em`
- Body color: `rgba(0, 0, 0, 0.9)`
- Paragraph side margin: usually `0 8px`
- Caption font size: `12px` or `13px`
- Caption color: `rgb(136, 136, 136)` or a nearby neutral gray

For articles that need a softer note-like feel, a looser rhythm is allowed, but the default reusable template should start from `17px / 1.75em / 0.034em`.

## 5. Emphasis Rules

Use emphasis to improve scanability, not to decorate every paragraph.

Recommended emphasis layers:

- Black bold: core judgment or sentence-level conclusion
- Brand-red bold: important data, pricing, growth result, strategic move, or business insight
- Underline: hard facts such as price ranges, product parameters, category expansion, dates, and named mechanisms
- Gray bold: author line, copyright note, source label, and image-source prefix

Default brand red:

```text
#b51e12
rgb(181, 30, 18)
```

Example inline styles:

```html
<span style="font-weight:bold;">核心判断</span>
<span style="color:#b51e12;font-weight:bold;">关键数据或商业结论</span>
<span style="text-decoration:underline;">价格、参数、品类或硬信息</span>
<span style="color:rgb(136,136,136);font-weight:bold;">图源：</span>
```

Rules of thumb:

- One paragraph should usually have at most one emphasized phrase.
- Use colored bold for the content that a reader should remember after skimming.
- Use underline for precise facts, not broad opinions.
- Do not stack color, underline, and bold on the same phrase unless it is a deliberate conversion module.

## 6. Founder And Team Visual Evidence

When an article uses a founder, creator, executive, or development team as part of its argument, the team section must include at least one identifiable, real image of that person or team. A product render, stock office image, AI-generated portrait, or anonymous conference crowd does not count as team evidence.

- Prefer, in order: an official team photo or creator portrait; a photo from the brand's own story/interview page; a reputable media or event portrait; a verified company-profile photo.
- Save the final asset in the product folder with a semantic filename such as `05_<product>_founder_<name>.jpg` or `05_<product>_team.jpg`.
- Every caption must identify the person/team, role, source, and—when an older historical photo is used—the time or original context. Do not present an old employer-era photo as a current startup team photo.
- If no credible founder/team image can be found, state that limitation in the research notes and do not fill the slot with an unrelated visual. The article may use a verified early product, workshop, or company-story image instead, but the caption must say what it is.

This rule applies across product observations, company profiles, and founder-led analysis. It exists to make team credibility visible and auditable, rather than decorative.

## 7. Article-Type Notes

For Kickstarter product observations:

- Use the universal `势差` banner. Do not add a Kickstarter-specific series label inside the GIF.
- Keep the article grounded in user pain points, product mechanism, campaign credibility, risk, and fit/non-fit audience.
- Add business-model or go-to-market analysis when the product has meaningful pricing, channel, DTC, creator, or crowdfunding signals.

For unicorn or company case studies:

- Use the universal `势差` banner. Do not add a unicorn-specific series label inside the GIF.
- Use brand-red bold for valuation, revenue, profitability, financing, and strategic turning points.
- Keep founder, investor, monetization, and competitor sections visually scannable.

For AI or thinking essays:

- Banner language should stay quieter.
- Use fewer cards and fewer colored highlights.
- Let paragraph rhythm and section titles carry the argument.
