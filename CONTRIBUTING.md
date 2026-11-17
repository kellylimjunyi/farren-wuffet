# Contributing to Pocket

Small improvements are welcome. Keep the tool easy to download, open and understand.

- Use fictional sample data only. Never submit real statements, transaction exports, names, account/card numbers, addresses, screenshots of personal finances, API keys or other secrets in code, issues or pull requests.
- Preserve the single-file, offline workflow. Opening `index.html` should not require a build step, account, network request, analytics service or external dependency.
- Keep claims honest. The current PDF picker is a mockup, and the user's own AI prepares JSON. Do not imply that a feature extracts documents or sends data unless that behavior is implemented and clearly explained.
- Cite official issuer sources for card-rule changes and record the date checked. Include rates, caps, exclusions, rounding and relevant eligibility conditions. Separate spending categories from verified rewards eligibility, and never encourage extra spending to earn miles.
- Check the affected behavior with fictional transactions, including caps, unknown eligibility and refunds where relevant. Verify that the page remains usable on mobile and with a keyboard.
- If you change the extraction prompt in `index.html`, update `prompts/statement-to-budget.txt` to match it exactly.

Explain what changed and how you checked it in your pull request. Keep the MIT notice with copies of the source.
