# Tacita Bugnath: writing portfolio

Technical writer at [Vestd](https://www.vestd.com), an FCA-regulated equity management platform, and the company's only writer. I write the help centre, in-app copy and customer emails for every product area, and I build AI workflows that keep that content accurate and up to date.

This repo collects samples of that work. Each one has a short note on the problem, what I did and what changed.

[LinkedIn](https://www.linkedin.com/in/tacita-bugnath) · tacita.bugnath@live.com

## Contents

1. [AI workflows](#ai-workflows)
2. [Help guides](#help-guides)
3. [In-app copy](#in-app-copy)
4. [Information architecture](#information-architecture)
5. [How I work](#how-i-work)

## AI workflows

| Sample | Problem | What I did | Result |
|---|---|---|---|
| [Product update sweep](ai-workflows/product-update-sweep/) | New features were shipping and help guides went out of date without anyone noticing. | Built an AI agent that checks each day's product updates against the help centre and reports which guides may need changing and where new guides are needed. It separates strong matches from weak leads and says what it couldn't check. | In its first three weeks it reviewed 18 updates and flagged 8 guides needing changes and 11 possible new articles. Within two weeks I'd updated 6 guides and written 3 new ones. |
| [Regulated content review skill](ai-workflows/regulated-content-review/) | Every guide needs the same checks before publishing, and in a regulated product a missed check is a compliance risk. | Wrote the review process as a Claude skill. It checks terminology, unhedged regulatory claims, readability, accessibility and how easily AI can retrieve the content, then gives a publish, expert sign-off or rewrite verdict. | On its first run it found a wrongly named accounting standard in a live help article. |
| [Guide request triage](ai-workflows/guide-request-triage/) | Guide requests came in through a slow form and had to be sorted by hand. | Replaced the form with a shared sheet that an AI agent scans daily. It creates Jira tickets and alerts me to new requests. | No manual triage, and data on which topics each business unit asks about most. |

## Help guides

| Guide | Why it's here |
|---|---|
| [Finding your documents on Vestd](help-guides/finding-your-documents.md) | Support flagged this as a common query. Related queries fell from around 25 a month to 5 in the month after it went live. |
| [How to upload your HMRC approval letter](help-guides/upload-hmrc-approval-letter.md) | Written after the support team's AI reply tool gave a customer wrong instructions, because no guide existed. Published within two weeks of the gap being flagged. |
| [How to exercise options on Vestd](help-guides/exercise-options.md) | A multi-step task guide for admins and option holders, covering both sides of the process. |
| [PISCES investor types](help-guides/pisces-investor-types.md) | Explains a new UK regulatory framework to investors who have to self-certify, without giving financial advice. |

More published guides: [How to upload share certificates](help-guides/upload-share-certificates.md) · [Identity verification and Companies House](help-guides/identity-verification.md) · [How to incorporate a company on Companies House](help-guides/incorporate-a-company.md)

## In-app copy

| Sample | What it shows |
|---|---|
| [Name change flow](in-app-copy/name-change-flow.md) | Before and after copy, plus design changes I proposed that the designer added: a confirmation summary and a card layout. |

## Information architecture

| Sample | Status |
|---|---|
| [Help centre reorganisation](information-architecture/help-centre-reorganisation.md) | In progress. An audit of every guide by category and a proposed new structure, so customers can find guides more easily. |

## How I work

- **I check everything AI produces.** The agents report what they couldn't verify, and nothing is published without a human review and, where needed, sign-off from a subject expert.
- **I use data to decide what to write next.** Support queries, guide requests, session replays and article performance.
- **I test what I document.** I follow my own steps on the platform and flag product and UX problems I find along the way.
- **I write for people and for AI.** Guides are structured so customers can follow them and AI assistants can retrieve the right answer.
