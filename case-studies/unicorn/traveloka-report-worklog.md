# Case Study: Traveloka Unicorn Financial Report

This document records the production workflow for the Traveloka weekly unicorn report and the iteration it added to the SOP.

## 1. Initial Topic

Company:

- Traveloka
- Indonesia / Southeast Asia
- Online travel platform, payments, PayLater, travel activities, and B2B inventory distribution

Final published title:

> 东南亚版携程赚钱了：Traveloka不想只做OTA

Core thesis:

> Traveloka is not only an OTA app for flights and hotels. Its more important question is whether it can turn local inventory, payments, fulfillment, support, and B2B distribution into Southeast Asia's travel-transaction infrastructure.

## 2. Title Iteration

The working title was more analytical:

> 东南亚版携程Traveloka：盈利之后，下一站是旅行基础设施？

The final title became more public-account friendly:

> 东南亚版携程赚钱了：Traveloka不想只做OTA

What improved:

- `携程` gives Chinese readers an immediate comparison point.
- `赚钱了` creates a clearer turning-point hook than a broad strategy question.
- `不想只做OTA` pulls the analogy back and states the article's real thesis.

Editorial lesson:

> A China analogy can be used as the hook, but the second half of the title should narrow the analogy and point to the company's real strategic difference.

## 3. Length Compression Iteration

The article became too long during research expansion because the same ideas appeared in multiple places:

- Traveloka is not only an OTA.
- It is moving toward infrastructure.
- B2B distribution is becoming more important.
- Public data is incomplete because the company is private.

The user feedback was that future drafts need stronger word-count discipline and should benchmark high-read comparable WeChat articles before finalizing length.

Reusable rule:

> For weekly unicorn business analysis, default to a tighter mobile-reading target of roughly 3,000-4,500 Chinese characters. Going beyond 5,000 characters requires clear incremental evidence, not repeated framing.

Cut first:

- repeated opening thesis lines
- duplicate market-size explanations
- repeated "not only X, but Y" transitions
- investor descriptions that do not change the investment logic
- risk paragraphs that restate earlier uncertainty without adding a new watch point

## 4. Narrative De-Duplication

The final draft showed that a long article can feel less rigorous when its logic repeats.

Better workflow:

1. Write a one-sentence logic spine before drafting.
2. Assign each section one job in that spine.
3. After drafting, mark every paragraph as `identity`, `evidence`, `model`, `investor`, `competition`, `risk`, or `judgment`.
4. Delete or merge paragraphs that repeat the same job without adding a new fact or implication.

For Traveloka, the smoother logic should be:

> Why Traveloka matters now -> what it is -> why Southeast Asian travel transactions are hard -> what data can and cannot be confirmed -> how money is made -> who is backing it and why -> where B2B and destination partnerships matter -> what risks remain.

Editorial lesson:

> Each section should answer a new reader question created by the previous section. If a section only restates the thesis, it should be shortened or removed.

## 5. User Voice Calibration

The user made many final copy edits. Those edits should become the voice sample for later articles.

Observed preferences:

- Shorter opening paragraphs.
- More direct judgment before detailed evidence.
- Less template language such as "核心结论," "三条主线," or "战略思考."
- Fewer AI-like summary phrases.
- A clearer rhythm of concrete fact -> business implication -> sharper question.
- Plain, conversational transitions instead of report-outline transitions.

Reusable rule:

> Before drafting the next article, compare the previous AI draft with the user's final edited version. Extract the user's cuts, replacements, and sentence rhythm. Treat those edits as the strongest style instruction.

## 6. English-Term Annotation

Traveloka used many English business terms and proper nouns:

- OTA
- App
- B2B
- API
- PayLater
- GMV
- cap table
- NDC
- East Ventures
- HBX Group
- Resorts World Sentosa
- Gyeonggi Tourism Organization
- Disney Cruise Line

The final editing rule is that the first occurrence of an English term should carry a Chinese explanation.

Examples:

- `OTA（Online Travel Agency，在线旅游代理平台）`
- `B2B（Business to Business，企业对企业）`
- `GMV（Gross Merchandise Value，平台成交总额）`
- `PayLater（先买后付/旅行分期）`
- `HBX Group（全球酒店分销与旅游科技集团）`

Editorial lesson:

> English terms can preserve professional precision, but the first appearance must lower the reading threshold for public-account readers.

## 7. Private-Company Data Framing

The Traveloka draft used a useful body-section pattern:

> 最新经营数据：能确认什么，不能确认什么？

This works better than hiding all uncertainty in the final source notes.

What it did:

- Confirmed public operating indicators such as app downloads, monthly active users, airline partners, accommodation supply, payments, profitability disclosures, and credit-facility repayment signals.
- Explicitly said what remained unavailable, including full audited 2025 financials, revenue, gross margin, net profit, operating cash flow, and PayLater bad-debt data.

Editorial lesson:

> For private-company articles with fragmented data, uncertainty can become a main-body section. This makes the analysis more credible and prevents overclaiming.

## 8. Investor Logic

Traveloka showed that investor sections need to separate equity investors from credit providers.

Different capital types in this case:

- East Ventures: local early-stage venture capital and founder-market fit.
- Expedia Group: strategic online-travel investor with hotel supply-chain relevance.
- JD.com, Hillhouse, Sequoia, and Global Founders Capital: growth and internet-platform capital.
- GIC and Qatar Investment Authority: long-duration sovereign wealth capital.
- INA, BlackRock, Allianz Global Investors, and Orion Capital Asia: private-credit or credit-facility providers during the post-pandemic recovery period.

Editorial lesson:

> Do not flatten all capital into "core investors." Equity investors, strategic investors, sovereign wealth funds, and private-credit providers imply different theses and different proof points.

## 9. Visual Iteration

Traveloka added several visual rules.

Title image:

- The first version was too visually busy.
- The better version separated the three core capabilities clearly.
- The Traveloka logo should appear as a transparent-background brand element, without an unnecessary decorative panel behind it.

Opening brand image:

- The first opening image overlapped too much with the business-network image.
- The better direction was a clean horizontal brand visual: central Traveloka logo, one or two slogan lines, and a few representative travel/payment elements.

Business network:

- The initial vertical network visual consumed too much mobile screen space.
- The final horizontal version preserved the logic while reducing reader drop-off risk.

Founder image:

- Real public founder photos were preferable to generic or generated founder visuals.

Reusable visual lessons:

- Separate the job of each image: cover image sells the thesis, brand image makes the company concrete, network image explains the operating system.
- Prefer horizontal layouts for complex business-network and competition visuals in WeChat long reads.
- Use real logos and real people only from sourceable assets; use generated images for abstract systems.
- Once a visual direction is approved, overwrite the standard referenced filename so the HTML remains stable.

## 10. Final Published Archive Lesson

The final WeChat-saved archive included many platform-generated images, SVG placeholders, QR codes, scripts, and opaque filenames.

Reusable rule:

> Do not use the final WeChat archive's raw `<img>` count as the body-image count. Use the production HTML for body-image validation, and use the saved WeChat archive only for post-publish review of title, layout, actual rendering, and platform artifacts.

## 11. SOP Changes Triggered by This Case

This Traveloka workflow added or strengthened these SOP rules:

- Add word-count benchmarking and length compression before final drafting.
- Add a narrative de-duplication pass so sections do not repeat the same thesis.
- Treat user final edits as the strongest voice-calibration sample.
- Require first-use Chinese annotations for English terms and acronyms.
- Allow a main-body `能确认什么，不能确认什么` section for private-company data uncertainty.
- Separate equity investors, strategic investors, sovereign capital, and credit providers.
- Separate the roles of title image, brand image, and business-network image.
- Prefer horizontal layouts for complex mobile infographics.
- Validate production HTML body images separately from final WeChat archive artifacts.
