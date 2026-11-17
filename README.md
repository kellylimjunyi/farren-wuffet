# Pocket — Budget & Miles

A small, free budgeting tool you can download and open in your browser. Bring your card statements to an AI you already use, review the results, and see your spending and an illustrative Singapore miles card plan.

**No coding, GitHub account, installation or bank connection is needed.** This is a working preview with sample data. A live hosted website has not been set up yet.

## Open Pocket in a few clicks

1. On this page, click the green **Code** button, then **Download ZIP**.
2. Unzip the downloaded folder.
3. Double-click **index.html** to open Pocket in a current browser, such as Chrome, Edge, Firefox or Safari.

You can also open [index.html](index.html) on GitHub and use **Download raw file** to download just that one file. The HTML contains everything the tool needs; keep the file and open it whenever you want to use it.

The sample month is fictional. Explore it first without sharing any statements.

## Use your own statements

1. **Get the prompt.** In Pocket, choose **Use my own AI** or **Get the AI prompt**, then copy or download the prompt. A plain-text copy is also available in [prompts/statement-to-budget.txt](prompts/statement-to-budget.txt).
2. **Use your chosen AI.** Download your credit/debit card statements as PDFs from your bank. Attach them to your own AI agent with the prompt. Remove personal identifiers first. Ask the AI to check transactions, repayments, refunds and possible duplicates against the statements, then return the reviewed JSON data. JSON is simply the structured text that Pocket can read; you do not need to write it yourself.
3. **Import and review.** Choose **Import & review data**, paste the returned JSON and import it. Check categories, your monthly budget and rewards eligibility. Then open **Plan my cards** to compare the available two-card and three-card illustrations.

Pocket currently handles **one calendar month in SGD** at a time. Unknown rewards eligibility stays out of the miles estimate until you verify it. A merchant name alone does not establish the merchant category code or payment channel used by a bank.

**PDF selection is a demonstration only.** Pocket does not read PDF contents, connect to an AI service, or extract transactions itself. Your own AI handles the PDFs, and you bring its reviewed JSON back into Pocket.

## Keep your work and share the tool

- Choose **Export my data** to save your reviewed transactions as a private JSON file. You can import that file's text in a later session.
- Changes exist only in the open page's memory. Closing or refreshing the page resets them, so export before leaving.
- Choose **Download clean HTML** to share a fresh sample-data copy of Pocket. This is separate from your private transaction export.
- Use **Reset demo** to return to the fictional example month.

The HTML makes no network requests and has no analytics, server, sign-in, API key or automatic data storage. Official bank reference links open external sites only when you click them. Any statements you attach to a separate AI service go to that provider and are subject to its settings and terms.

## What the card planner covers

The current candidate set is deliberately small:

| Card | Illustrative role |
| --- | --- |
| DBS Woman's World | Eligible online retail spending |
| UOB Lady's World | Eligible dining with Dining selected |
| Citi PremierMiles | Other eligible SGD spending |

This is a limited allocation illustration, not an exhaustive search for the best card in Singapore or a calculation of miles already awarded. It routes whole purchases within the model's caps, applies its stated rounding assumptions, and compares gross miles before fees. Actual rewards depend on issuer rules, exclusions, posting dates, merchant codes, payment channels and your eligibility.

The planner includes source links and conditions; its rules were checked on **17 November 2026**. Recheck official terms before relying on a plan. Fees, interest, welcome offers and airline redemption availability are not included in the miles totals. Refunds pause miles estimates because this preview cannot match them to their original rewards.

Keep your budget first. Earning miles should not require extra spending or carrying a card balance.

## Make it your own

Pocket is plain HTML, CSS and JavaScript in [index.html](index.html), with no build step or dependencies. You can ask your own AI coding agent to adapt it, inspect the calculations, add supported cards or change the design.

Use fictional examples when sharing a change. Never put real statements, transaction exports, personal details or API keys in this public repository. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

Original code is available under the [MIT License](LICENSE). Bank names identify their products; Pocket is not affiliated with those banks.
