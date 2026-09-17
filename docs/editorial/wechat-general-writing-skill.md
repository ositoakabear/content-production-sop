# General WeChat Writing Skill

This skill applies to Axiong's WeChat essays across topics. Use it with `wechat-editorial-style-guide.md` and the relevant project-specific playbook.

## 0. Non-Duplication Rule

Before adding a new rule to this repository, check whether the same rule already exists.

Already-covered rules should not be repeated here:

- Basic WeChat visual identity and typography: `wechat-editorial-style-guide.md`
- General HTML packaging, inline styles, local image paths, and image validation: `../../playbooks/unicorn/unicorn-financial-report-sop.md`
- Generated-image safety, raw asset backup, crop-safe title images, and caption strategy: `../../case-studies/unicorn/rappi-report-worklog.md` and `../../case-studies/unicorn/kavak-report-worklog.md`

If a new rule conflicts with an existing rule, do not overwrite the existing SOP directly. Prepare the difference for owner review first.

## 0.1 Growth-Optimization Gate

Every WeChat writing task that says it follows this repository must also use `content-growth-optimization-standard.md`.

Before finalizing the article:

- Apply every relevant optimization item in that standard.
- If an item is intentionally not used, state the reason and remind the owner to review the exception.
- Do not treat candidate insights in `social-media-methodology-observation-log.md` as approved rules before they pass the three-cycle evidence gate and owner review.

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


## 8. Finished Article Delivery Package（成稿交付包）

生效日期：2026-09-17。以下为作者明确要求的通用交付规范，适用于各栏目；不属于从单篇表现推导的增长结论。

每篇成稿默认同时交付以下五项，不能只交正文或只交制作计划：

1. **富文本 HTML（超文本标记语言）**：提供可预览、可复制的成品与纯正文文件；正文使用内联样式，复制区不包含标题备选、导语字段、广告建议、按钮和内部备注。具体排版、图片及平台约束继续引用现有规范。
2. **标题图**：交付最终图片文件，至少包含公众号横版约 2.35:1 与方形 1:1 版本；逐一检查文字、主体和裁切安全区。封面文字层级遵循通用视觉规范，不以提示词代替图片。
3. **导语**：单独交付一段可直接用于摘要的中文导语，默认约 50—100 字；交代对象、变化和阅读价值，不能把未经证实的结论写成点击承诺。导语与正文首段可相近，但不要机械重复展示。
4. **广告类型和靠前位置建议**：单列首选、备选位置、匹配类型、选择理由和排除项；优先寻找靠前的完整价值单元结束处，给出前后文字锚点。具体位置与广告限制统一以 `content-growth-optimization-standard.md` 第 4.6 节为准，不在正文放空广告框。
5. **英文术语括号中文解释**：面向读者的标题、导语、正文、图注、图片文字及交付建议中，凡保留英文术语、缩写或英文专名，均在其后用全角括号给出中文含义、通行译名或角色说明，如 `API（应用程序编程接口）`、`Ontology（业务本体，即企业对象及其关系）`、`Palantir（帕兰提尔，美国企业数据与决策软件公司）`。每次保留英文均带释义，重复过密时改用中文简称；不以“读者熟悉”省略解释。标题及封面优先用中文减少拥挤。原始网址、文件路径和程序代码不改写。固定文案出现英文时，仅补括号释义，不改动其他措辞。本条替代栏目规范中“后续可省略释义”或“知名品牌免释义”的宽松处理。

交付前核对五项齐全、链接可用、图片文件完整，并明确素材完成、草稿保存、文章正式发布和规范仓库发布各自的真实状态。仅获得仓库发布授权时，不将文章同步发布到外部平台。
