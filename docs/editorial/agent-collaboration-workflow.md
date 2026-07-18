# Codex + Claude Code Collaboration Workflow

This workflow defines how Codex and Claude Code should cooperate on future public-account articles without creating two layers of generic AI prose or wasting model budget.

## 1. Default Division Of Labor

Use this default order for data-heavy business articles, especially `每周独角兽观察`:

1. **Codex drafts first.**
   Codex reads the local SOP, prior edited drafts, source boundaries, article package structure, and publishing constraints. It produces the first WeChat-ready draft with clear facts, source caveats, title direction, recurring series labels, and the `资料口径` block.

2. **Claude Code red-teams once.**
   Claude Code should not rewrite the full article by default. It should act as a cold editorial reviewer: identify weak openings, repeated logic, AI-like phrasing, overcertain private-company claims, title problems, and sections that can be cut without losing meaning.

3. **Codex finalizes.**
   Codex decides which Claude Code suggestions to accept, protects factual and valuation wording, updates the Markdown/HTML package, validates images and rich-copy HTML, and produces the final publishing artifact.

Short name:

> Codex 主笔，Claude 红队，Codex 定稿。

## 2. When To Reverse The Order

Claude Code may draft first only when the piece is mainly a personal essay, interview reflection, AI thinking note, or low-data narrative where mood and prose rhythm matter more than source boundaries.

For financial, unicorn, product, company, or valuation articles, Codex should draft first because these drafts depend on claim hygiene, local publishing conventions, source notes, and package validation.

## 3. File Handoff Convention

For each article, keep the handoff small and auditable:

```text
<company>-research-brief.md
<company>-draft-v1.md
<company>-editorial-review-by-cc.md
<company>-final.md
<company>-wechat.html
<company>-wechat-rich-copy.html
images/
```

Do not ask Claude Code to read the whole repository unless the article genuinely requires it. Give it only the draft and the style/editing criteria.

## 4. Claude Code Budget Rules

Claude Code can be expensive. Use it as an editor, not a second writer.

- Run at most one review pass by default.
- Send only the current draft plus the review prompt, not the whole research archive.
- Ask for findings and suggested local edits, not a complete rewrite.
- Cap the output to a compact review: `必须改 / 建议改 / 可保留`.
- For small articles, skip Claude Code unless the draft feels structurally weak.
- Never let Claude Code rewrite source notes, financial claims, valuation dates, or legal caveats without Codex rechecking them.

## 5. Standard Claude Code Review Prompt

Use this prompt when asking Claude Code to review a WeChat business-analysis draft:

```text
你是微信公众号商业分析编辑，不要重写全文。
请审阅这篇“每周独角兽观察”草稿，只输出修改建议。

目标：让文章更像一个有经验的人类商业编辑写的，而不是 AI 总结稿。

重点检查：
1. 开头是否足够快进入核心判断
2. 哪些段落重复或像 AI 总结
3. 哪些判断可以更锋利
4. 哪些事实表述可能过度确定
5. 标题是否更适合公众号
6. 哪些段落可以删除或合并
7. 结尾点评是否有作者判断，而不是复述正文

请按“必须改 / 建议改 / 可保留”三类输出。
每条建议尽量短，并说明对应段落或小标题。
不要直接生成新稿，不要全文改写。
```

## 6. Codex Finalization Checklist After Claude Code Review

After Claude Code returns comments, Codex must:

- Accept only suggestions that improve reader clarity, judgment strength, or voice.
- Reject suggestions that weaken claim hygiene or blur source uncertainty.
- Keep series labels stable: `每周独角兽观察` and `每周独角兽观察员点评`.
- Recheck valuation dates, revenue/profit wording, and private-company caveats.
- Remove any new AI-like transition introduced during revision.
- Update both Markdown and HTML if both exist.
- Validate all local image paths and rich-copy HTML before publishing.

## 7. What Not To Do

- Do not run alternating full rewrites between agents.
- Do not use Claude Code to polish every paragraph line by line unless the user explicitly asks.
- Do not let Claude Code add unsupported facts or stronger certainty than the sources allow.
- Do not send large image folders, generated assets, or published WeChat archive files to Claude Code for a text-only review.
- Do not treat a smoother draft as automatically better if the judgment becomes less specific.
