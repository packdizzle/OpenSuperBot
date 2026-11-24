# Affiliate operations teammate

OpenSuperBot includes an **Affiliate Ops** teammate for organizing campaign details, summarizing operator-supplied reports, and preparing promotional drafts. It is intentionally not an automated Stake or Syztmz integration.

## Set up

1. Start the gateway so the bundled `teammates/affiliate-ops` teammate is seeded.
2. In **AI models**, choose the teammate's model. To use Grok 4.7, configure an authorized xAI API connection using the app's existing model setup; do not put API keys in the repository or teammate files.
3. Keep the affiliate code and dashboard-generated campaign URLs in the teammate's private local `memory/affiliate-settings.md`, not in this repository. The settings file can also record the source and date for verified terms. The supplied affiliate code is deliberately not stored in tracked files. Store credentials only through the app's existing Models, Connectors, or local Vault flows.
4. Export reports manually from each partner dashboard where permitted, then attach or provide them to the teammate. Use aggregate campaign totals only; remove player names, handles, contact details, account identifiers, and individual wager histories first.

Keep Stake direct-affiliate and Syztmz sub-affiliate reporting separate. Use only campaign URLs copied from the relevant official dashboard; the assistant will not construct a tracking URL from a code or assume that a referral or reward is shared across programs.

## Reports and drafts

For useful comparisons, provide each report's program, campaign, report period, export timestamp, currency, and aggregate metrics (for example: clicks, signups, qualified-referral count, and reported commission). Definitions can differ between partners, so the teammate should flag rather than combine non-comparable metrics. If a report is stale or a period is missing, the summary should say so.

Promotional copy and any proposed reward or campaign change remain drafts. The teammate must show the exact draft, intended audience or destination, and its factual sources, then hold it for explicit human approval. A human must verify terms, audience eligibility, the tracking URL, and jurisdiction requirements before using it. Affiliate disclosures must be clear and adjacent to links or codes; gambling-related copy must include responsible-gambling language and must not target minors or vulnerable people.

## Integration status and limits

The public Syztmz Affiliates page describes campaigns and a dashboard, but no public developer/API documentation was found. Consequently, this MVP does not connect to Syztmz or Stake, scrape authenticated pages, or automate attribution or rewards. Use a permitted manual export until the program provides verifiable integration documentation and authorization.

Affiliate marketing and gambling rules vary by jurisdiction, and partner terms may restrict campaigns or automation. Review both applicable local requirements and current Stake/Syztmz terms before running promotions. This assistant does not place bets, manage gambling accounts, or move money.
