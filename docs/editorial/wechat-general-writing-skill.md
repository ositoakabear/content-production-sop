# General WeChat Writing Skill

This skill applies to Axiong's WeChat essays across topics. Use it with `wechat-editorial-style-guide.md` and the relevant project-specific playbook.

## 0. Non-Duplication Rule

Before adding a new rule to this repository, check whether the same rule already exists.

Already-covered rules should not be repeated here:

- Basic WeChat visual identity and typography: `wechat-editorial-style-guide.md`
- General HTML packaging, inline styles, local image paths, and image validation: `../../playbooks/unicorn/unicorn-financial-report-sop.md`
- Generated-image safety, raw asset backup, crop-safe title images, and caption strategy: `../../case-studies/unicorn/rappi-report-worklog.md` and `../../case-studies/unicorn/kavak-report-worklog.md`

If a new rule conflicts with an existing rule, do not overwrite the existing SOP directly. Prepare the difference for owner review first.

## 1. Author Voice

For Axiong's own essays, preserve the author's thinking habits instead of polishing everything into a generic media voice.

Preferred:

- Start from a concrete personal trigger before moving to abstract judgment.
- Keep first-person doubt, self-positioning, and admitted partial understanding when they build trust.
- Use plain but slightly sharp sentences.
- Let questions push the argument forward instead of making the ending sound mysterious.
- Offer several rewriting options by tone when the user is choosing wording.

Avoid:

- Repeating the same grand question in multiple sections.
- Hollow philosophical phrasing that feels like `故弄玄虚`.
- Overusing "终极价值" style language when a concrete distinction would work better.
- Forcing a technical-authority posture when the author wants to write as a thoughtful ordinary person.

Useful concrete distinction patterns:

```text
什么只是技能，什么才是能力。
```

```text
哪些能力会被工具接管，哪些能力会变得更重要。
```

## 2. Series-First Planning

When an idea may become a series, plan the series before overloading article one.

Recommended planning fields:

- Series name
- Four to six article titles
- One-sentence role of each article
- Which personal examples belong to which article
- Which theory, book, or technical concept should be used lightly rather than becoming the main axis

Article one should usually work as the doorway:

- Introduce the personal trigger.
- Explain why the issue matters now.
- Give enough context for new readers.
- Leave one clearly defined question for article two.

Do not try to answer the whole series in the first article.

## 3. Series Title Layering

For multi-part essays, prefer a stable series title plus issue number plus article-specific title.

Pattern:

```text
<系列名>｜<编号>：<本篇标题>
```

Keep three title layers separate:

- `WeChat title`: carries the full click promise.
- `Cover image text`: can be much simpler, often only the series name and issue number.
- `Digest`: states the core discomfort or question in one plain sentence.

Avoid putting the whole article title into the cover image when the WeChat title already carries it.

## 4. Ending And NEXT Blocks

The final body section and the `NEXT` block should not do the same job.

Use the final body section to close the current article's argument.

Use the `NEXT` block to hand the reader to the next article's specific question.

If both sections ask "人还剩下什么" or another broad existential question, revise one of them into a concrete transition.

## 5. Rich Text Editing Additions

Do not repeat the existing HTML packaging rules. This section only records additions from recent editing experience.

When generating a copy-helper HTML page:

- Keep a clean copy root, such as `#copy-root`, that contains only article content.
- Do not put title, digest, internal notes, or copy buttons inside the copyable article area.
- Maintain source HTML and copy-helper HTML separately when useful.
- Do not place screenshot-only editing notes into the final article body.
- If the user still wants to insert text, GIFs, or images manually, leave an intentional blank paragraph before the relevant section.

Recommended blank editing line:

```html
<p style="margin:0 8px 24px;min-height:1.75em;"><br /></p>
```

## 6. Visuals As Thinking Tools

Use visuals when they clarify thinking, not just to decorate the article.

Good use cases:

- A concept that readers may wrongly understand as a single straight line
- A series identity cover
- A comparison framework
- A transition between article one and later articles

For thinking essays, prefer minimal visuals and fewer decorative elements. Keep precise labels in editable text or captions unless the image text has been visually checked.

## 7. Typography Change Gate

The approved general typography default lives in `wechat-editorial-style-guide.md`.

Future typography changes should still be reviewed before they replace the recorded WeChat defaults.
