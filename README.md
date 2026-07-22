# Content Creation Playbook

This repository collects reusable content-production playbooks, editorial standards, platform packaging rules, case studies, and automation skills for WeChat and Xiaohongshu publishing.

It is organized as a shared knowledge base for the public account "势差": universal rules live in `docs/`, vertical-column methods live in `playbooks/`, executable agent skills live in `skills/`, reusable scripts live in `scripts/`, and production retrospectives live in `case-studies/`.

## Universal Standards

- `docs/editorial/content-growth-optimization-standard.md`
  Mandatory growth-optimization gate for every WeChat task that follows this repository: first-screen delivery, factual reliability, title packaging, conversion, baseline growth, and feedback collection.

- `docs/editorial/social-media-methodology-observation-log.md`
  Evidence log for candidate operating methods. Candidates require three independent weekly or monthly review cycles and owner approval before becoming formal methodology.

- `docs/editorial/social-media-reporting-standard.md`
  Weekly, monthly, and quarterly reporting requirements, including mandatory Traffic Master revenue analysis and missing-data reminders.

- `docs/editorial/wechat-editorial-style-guide.md`
  Visual identity, universal opening banner, mini-program entry placement, typography, and emphasis rules for "势差".

- `docs/editorial/wechat-general-writing-skill.md`
  Reusable author voice, series-first planning, title layering, endings, and rich-copy additions for WeChat essays.

- `docs/editorial/agent-collaboration-workflow.md`
  A cost-aware Codex + Claude Code workflow for drafting, red-team review, and finalization.

- `docs/platforms/wechat-rendering-and-api-pitfalls.md`
  WeChat HTML rendering constraints, draft API pitfalls, image upload rules, IP whitelist notes, encoding issues, and Windows execution notes.

- `docs/platforms/xiaohongshu-adaptation.md`
  Reusable Xiaohongshu adaptation rules for turning long-form material into a short mobile-native post.

- `docs/assets/image-asset-workflow.md`
  Local image package conventions, naming rules, source/rejected asset folders, and cover/body image validation.

## Vertical Playbooks

- `playbooks/unicorn/`
  SOP and accumulated lessons for `每周独角兽观察`: private-company claim hygiene, financial and operating analysis, investor logic, competitor modeling, source notes, and final voice calibration.

- `playbooks/kickstarter/`
  SOP and accumulated lessons for Kickstarter product observations: product pain-point writing, founder and campaign credibility, product assets, competitor cards, risk notes, Xiaohongshu adaptation, and WeChat packaging.

- `playbooks/ai-boundary/`
  Project-specific structure, tone guardrails, theory boundaries, and visual preferences for the `AI 的边界` series.

## Automation Skills And Scripts

- `skills/cursor/kickstarter-wechat-post/`
  Imported Cursor Agent skill for turning Kickstarter-style product material into a WeChat draft and Xiaohongshu post.

- `scripts/wechat/publish_wechat.py`
  Reusable WeChat draft publishing script copied out of the Kickstarter skill so it can serve other article types too.

## Case Studies

- `case-studies/unicorn/`
  Production worklogs and retrospectives for Kavak, Rappi, Uala, Traveloka, and the cross-article unicorn workflow progression.

## Repository Maintenance

- Keep universal rules in `docs/`; do not duplicate them inside every vertical playbook unless the rule has a column-specific variation.
- Treat `content-growth-optimization-standard.md` as a mandatory gate whenever a task says it follows this repository. Apply the relevant items or explicitly ask the owner to review any intentional exception.
- Update `social-media-methodology-observation-log.md` only through formal weekly or monthly reviews. Do not promote a candidate before three independent cycles and owner approval.
- Include Traffic Master revenue and monetization analysis in every weekly, monthly, and quarterly report. If data is missing, ask the owner for the available backend export or screenshots before finalizing.
- Keep vertical methods in `playbooks/<column>/`; each playbook should explain what is specific to that article type.
- Keep executable agent skills in `skills/`; skills can reference shared docs, but should remain installable.
- Keep one-off production notes in `case-studies/`; promote repeated lessons into `docs/` or `playbooks/`.
