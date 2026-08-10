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

- `source/`: untouched official product, brand, founder, public-source, or media originals used as inputs. Preserve the highest-resolution file available rather than overwriting it with a crop or compressed export.
- `raw-generated/`: raw AI-generated or generated-diagram outputs.
- `rejected-<reason>/`: rejected directions worth preserving because they teach a reusable lesson.

Do not preserve throwaway temporary crops unless they explain a production decision.

## Title-Cover Copy

- A standard title cover contains only the column label and the subject or product name.
- Do not add a slogan, core selling point, feature phrase, emotional hook, campaign result, or duplicate article headline.
- For Kickstarter product observations, use `本周好物观察` plus the official product name only.
- Keep both required text levels legible in the intended horizontal cover. Treat extra copy as an error during visual QA.

## Title-Cover Canvas And Crop Safe Area

The canonical WeChat title-cover canvas is `2.35:1`.

- Recommended working export: `1200 x 511` or another true `2.35:1` equivalent.
- The centered `1:1` square is the mandatory safe area. On a `1200 x 511` canvas, use the centered `511 x 511` square as the crop check.
- Keep the primary visual subject and every required text element inside the central square. Decorative background, secondary objects, and atmosphere may extend into the left and right wings.
- Check two previews before approval: the full `2.35:1` image and the centered `1:1` crop.
- A cover fails QA if either crop cuts through the product, face, identifying logo, column label, or subject/product name, or if the square crop loses the main visual hierarchy.
- When a separate square asset is needed, derive it from the approved safe master; do not rebuild a composition with a different subject or message.

Vertical playbooks inherit this geometry. A project may create extra platform-specific derivatives, but it must not replace the `2.35:1` title cover or weaken the central `1:1` safe area without an explicit owner exception.

## Image-Source Priority

For any image that represents a real product, person, company, interface, location, event, or document, use the following order:

1. **First-party official original**: official website, product page, crowdfunding campaign, press kit, newsroom, investor-relations page, official store, official social account, or the creator's own story page.
2. **Credible public or media original**: a reputable interview, event page, filing, platform page, or media report when no suitable first-party asset exists or when the external context is itself relevant.
3. **Generated visual**: only when no suitable real asset can be obtained, or when the image's job is explicitly conceptual, such as an abstract system, scenario composite, business-model explanation, or clearly labeled illustration.

Acquisition and handling rules:

- Search the official domain and official campaign page first. Image search may help discover an asset, but follow it back to the original source page before downloading.
- Prefer the original downloadable file or the highest-resolution official version. Use a screenshot only when the interface or page context is the evidence, or when no original file is available.
- Never replace an available official product image with a generated look-alike merely for visual consistency.
- Real founders, teams, executives, products, logos, UI screens, documents, and event scenes require real-source assets. Do not invent or reconstruct them with generative AI.
- If a generated illustration is used because real imagery is unavailable, keep it visibly illustrative, label it `示意图` in the caption, and do not imply that it is an official product render or documentary image.
- Preserve an untouched source copy and record the source page in the caption, source log, or article notes. Do not remove watermarks or source marks to make a public image appear first-party.
- Crop, color-correct, or compose only in a derivative file. The source original remains auditable in `source/`.

## Visual Integrity Rules

- Do not generate fake founder or team photos.
- Do not fake official logos or UI screenshots.
- Use real product images when readers need to inspect the product.
- Generated visuals are best for abstract systems, scenario composites, or clearly labeled diagrams.
- Keep accurate text in HTML captions when possible instead of baking fragile text into images.
- Do not use generation as a shortcut around source research. The visual form must match the evidentiary job of the image.

## Validation

Before publishing:

- Confirm every body `<img src>` points to an existing local file or an uploaded WeChat CDN URL.
- Validate cover/share images separately from body images.
- Confirm the title cover is `2.35:1` and that all essential content survives the centered `1:1` crop.
- Preview on mobile.
- Check paired images for correct order.
- Check that captions and source notes match the actual image.
- Confirm real products, people, logos, UI, events, and documents use official or credible public-source originals rather than generated substitutes.
- Confirm each downloaded public image can be traced back to its source page and that the untouched original remains in `source/` when the package uses a source folder.
