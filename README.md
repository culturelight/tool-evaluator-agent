# Tool Evaluator Agent · 工具評估卡

A personal AI instruction project by **B Hui** for evaluating physical tools, software, AI, and workflows through **decision quality, economics, and governance**.

It guides an AI assistant to produce a structured 15-section evaluation card: what the tool does, who retains control, how results are checked, annual value and cost, alternatives, and when to stop using it.

## Use it

Open [Tool Evaluator Agent in ChatGPT](https://chatgpt.com/plugins/plugin_54500a323f148191af4c600ddae1d8b3?open_in_app).

Copy [the Traditional Chinese instructions](INSTRUCTIONS.zh-Hant.md) into an AI assistant that supports custom instructions, then provide the tool name, users, frequency, costs, expected lifespan, and one or two intended uses. The instructions retain some Cantonese phrasing.

Missing information should be marked **Unknown** or presented as a justified range. Estimates use conservative values: lower benefits and higher costs, with numbered assumptions, currencies, units, and formulas.

Suggested requests:

- 「評估：Notion AI，15人每日用」
- 「評估：新 CRM，含替代方案與 Stop Rule」
- 「評估：報銷流程自動化工具，估算 breakeven」

These are starter prompts, not measured demonstrations.

## Worked example

Read [the OpenAI Codex evaluation card](examples/openai-codex.zh-Hant.md) for a complete Traditional Chinese example with all 15 sections, exactly two use cases, alternatives, governance, numbered assumptions, and conservative cost calculations.

The example is dated **2026-10-07**. It uses an illustrative single-user scenario, not measured productivity results: conservative annualized cost is **USD 2,080**, estimated annual time value is **USD 960**, and estimated annual net value is **−USD 1,120**. At the assumed value rate, the break-even threshold is about **2.17 hours saved per week** over 48 working weeks. Check current product terms and replace the assumptions with your own recorded costs and outcomes before deciding to adopt or renew.

## What makes it useful

- Exactly two use cases, with human judgment and verification points.
- Annual costs covering subscriptions, setup, training, operations, and risk allowances.
- Named owners and approvers, review dates, fallback procedures, and stop rules.
- An explicit alternative that works without the proposed tool.

## Interpretation and limitations

This repository shares a prompt specification, not executable software or a validated financial model. Outputs depend on the model, inputs, and available evidence; the supplied review's star ratings are not published as performance results.

Check calculations independently. Time saved is an estimated benefit, not automatically a cash saving. For cash payback, distinguish recurring net cash benefits from accounting costs: do not subtract amortized setup costs and then count those same setup costs again as the initial investment. If benefits or costs cannot be supported, retain Unknown rather than treating an estimate as evidence.

The original 15-section specification is preserved. Its annual net-value comparison and simple payback formula require this interpretation. Human reviewers remain responsible for adoption and renewal decisions.

## 中文簡介

用一張工具評估卡，檢視工具的用途、成本、效益、核驗方式、治理責任與停用條件。資料不足時列明 Unknown 或假設區間；比較替代方案時，必須包括「無此工具」的做法。

核心理念：工具可以不達到損益平衡，但不應把判斷權交給工具。

完整示例：[OpenAI Codex 工具評估卡](examples/openai-codex.zh-Hant.md)。示例包含來源、成本公式與假設清單；估算不代表實測成效。

## Copyright

See [COPYRIGHT.md](COPYRIGHT.md) for use of this project's authored material.
