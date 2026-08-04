# Image Asset Workflow

Use this guide for WeChat, Xiaohongshu, and supporting visual packages.

## Folder Conventions

Each article or product should have a local asset folder that survives after publishing.

For Kickstarter products:

```text
.../Kickstarter/<ProductName>/
```

For company case studies:

```text
.../<Column>/<Company>/
  images/
    source/
    raw-generated/
    rejected-<reason>/
```

## Naming Rules

Use numbered semantic filenames so image order is obvious during mobile preview:

```text
01_title_cover.jpg
02_lifestyle_or_identity.jpg
03_founder_or_team.jpg
04_business_or_feature_diagram.jpg
05_competitor_or_scenario.jpg
06_transition.gif
```

## Source, Generated, And Rejected Assets

- `source/`: official product, brand, founder, public-source, or media images used as inputs.
- `raw-generated/`: raw AI-generated or generated-diagram outputs.
- `rejected-<reason>/`: rejected directions worth preserving because they teach a reusable lesson.

Do not preserve throwaway temporary crops unless they explain a production decision.

## Title-Cover Copy

- A standard title cover contains only the column label and the subject or product name.
- Do not add a slogan, core selling point, feature phrase, emotional hook, campaign result, or duplicate article headline.
- For Kickstarter product observations, use `本周好物观察` plus the official product name only.
- Keep both required text levels legible in the intended horizontal cover. Treat extra copy as an error during visual QA.

## Visual Integrity Rules

- Do not generate fake founder or team photos.
- Do not fake official logos or UI screenshots.
- Use real product images when readers need to inspect the product.
- Generated visuals are best for abstract systems, scenario composites, or clearly labeled diagrams.
- Keep accurate text in HTML captions when possible instead of baking fragile text into images.

## Validation

Before publishing:

- Confirm every body `<img src>` points to an existing local file or an uploaded WeChat CDN URL.
- Validate cover/share images separately from body images.
- Preview on mobile.
- Check paired images for correct order.
- Check that captions and source notes match the actual image.
