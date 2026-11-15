# Contributing to the Deploy@EU Case Library

Thank you for sharing what you learned. This page explains what we accept, how to submit, and how review works.

## First contributions

You don't need a full case to start. Any of these counts as a contribution and is credited:

- **Recommend an interview guest** — someone who has deployed AI in a European company and could talk about it (open an issue: *Guest recommendation*).
- **Fix or complete an existing case** — a typo, a broken link, a missing detail the author agrees to add.
- **Report a wall** — "We could not connect system X / the works council stopped Y / GDPR blocked Z." Open an issue: *Wall report*. Walls that come up again and again become topics for talks and shared tools.
- **Recommend an article** for a reading session.
- **Translate** a case summary into English, German, French or another language.

A maintainer will answer within **48 hours**.

## Let your AI help

Copy this into ChatGPT, Claude or any assistant that can read web pages:

> Help me write a Deploy@EU case and member profile: https://deploy-eu.github.io/write-a-case.txt

It will interview you, fill in the template, check the rules below, and give you finished files to submit.

## Other ways to share a case

- **Be interviewed.** Tell a maintainer you have a story, or recommend yourself with a *Guest recommendation* issue. We talk for 30–45 minutes, write the case from the conversation, and you approve it before anything is published. If you agree, the talk can also become part of our interview series.
- **Use a pseudonym.** Your real name never has to appear. Companies are always anonymised unless they agreed to be named.
- **Only a few lines?** Send them anyway. A maintainer decides whether they can be published as they are, or helps you turn them into a full case.

## Add yourself

Your profile lives in [`members/`](members/) as one file, `members/<your-github-handle>.md` (copy [`members/_TEMPLATE.md`](members/_TEMPLATE.md)). Your cases live in your own folder, `cases/<your-github-handle>/`. The website reads both folders automatically, so once a maintainer merges your files you appear on https://deploy-eu.github.io with your name on your cases.

No GitHub account, or no time to learn Git? Open a **Member profile** or **Case submission** issue and paste the text, or send it to any maintainer. We add the files for you, with you as the author.

## Writing a case

1. Copy [`cases/_TEMPLATE.md`](cases/_TEMPLATE.md) to `cases/<your-github-handle>/YYYY-MM_short-title.md`. Each contributor (or team) gets their own folder; add a short `README.md` there about yourself if you like. The website picks up every case automatically and shows you as the author.
2. Fill in every section you can. Short is fine; honest is required.
3. Open a pull request. Or, if you don't use Git, open a **Case submission** issue and paste your text — a maintainer will turn it into a pull request with you as author.

Translations: you may add `title_xx`, `summary_xx` and `industry_xx` fields (xx = zh, de, fr, it, es) to the front matter so the website shows your case card in that language. Your AI can write them; maintainers add missing ones during review.

Language: English preferred. German, French and other languages are welcome; a maintainer will help add a short English summary.

## Wall tags

Use these tags in the `walls:` field of a case and in wall reports, so we can see which walls come up most often. Add a new tag only if none fits.

| Tag | Meaning |
|---|---|
| `no-api` | The system has no API, or only manual exports |
| `legacy-desktop` | Old on-premise / Windows software that has to be operated through its interface |
| `data-quality` | Messy, inconsistent or missing data (e.g. the same product under three names) |
| `gdpr` | Data-protection questions (consent, processors, data location) |
| `ai-act` | EU AI Act questions (risk class, transparency, documentation) |
| `works-council` | Works council (Betriebsrat) involvement or agreement needed |
| `change-management` | People did not adopt it, or the process owner changed |
| `vendor-lock` | The software vendor blocks or charges for access |
| `cost` | Running costs (tokens, licences, infrastructure) became a problem |
| `reliability` | The automation broke silently or too often |

## What we accept

| ✅ Yes | ❌ No |
|---|---|
| Real deployments you worked on (live, pilot or stopped) | Product announcements, pitches, "book a demo" |
| Failures and abandoned projects — often the most useful | Prices, rates, sales contacts |
| Measured results; estimates clearly labelled | Unverifiable claims ("10x productivity") |
| Vendors and tools named factually | Rankings or recommendations of vendors |
| Anonymised companies, or named with their consent | Personal data, client data, confidential documents |

The community does not endorse any company — including sponsors and members' own businesses. Mentioning that you built something is fine; turning the case into an advertisement is not.

## Review

Every case is reviewed by one maintainer who did not write it. The checklist is in the pull request template:

1. **Consent** — whoever needed to agree to publication has agreed.
2. **No personal or confidential data** — names of private persons, emails, client figures, internal documents removed.
3. **Honest numbers** — measured vs estimated is clear.
4. **No advertising** — no prices, no sales contacts, no "we are the best".
5. **Useful** — "where it got stuck" says something concrete.

Review is about these five points, not about style. If something needs to change, the reviewer explains why; you can always disagree and ask another maintainer.

## Credit

Merged contributions are recorded and you are added to [CONTRIBUTORS.md](CONTRIBUTORS.md). How recognition works (badges, roles, honours) is described in [RECOGNITION.md](RECOGNITION.md). There are no points and no leaderboards.

## Your data

We record contributions (date, type, link, who confirmed) so we can credit people. Only you and the management team can see your full record; publicly visible are your name, your credited work and the badges you choose to show. You can ask for your record or for its deletion at any time. See [RECOGNITION.md](RECOGNITION.md#privacy).
