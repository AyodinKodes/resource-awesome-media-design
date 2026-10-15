# CLAUDE.md

## Project

- An awesome list of tools, places and resources for media design.
- Source: post-its from the first-year Master Media Design students, HEAD – Genève, Tech Corner, session 2 (9 October 2026).
- Use in class: session 3 (16 October 2026) teaches forks, pull requests and issues with this repository.
- The students are not members of the organisation. They fork from their own GitHub accounts.
- Repository: https://github.com/HEAD-MasterMediaDesign/resource-awesome-media-design (public, CC0 1.0).

## Files

- `README.md`: the list. The checks lint only this file and `contributing.md`.
- `contributing.md`: rules and steps for students (website and terminal).
- `.github/pull_request_template.md`: the checklist in each new pull request.
- `.github/workflows/checks.yml`: the `awesome-lint` and `link-check` jobs.
- `.lycheeignore`: URLs that the link check skips.
- `LICENSE`: CC0 1.0.

## Awesome list conventions

Follow the [awesome manifesto](https://github.com/sindresorhus/awesome/blob/main/awesome.md) and the [list checklist](https://github.com/sindresorhus/awesome/blob/main/pull_request_template.md). Main rules:

- The title is `# Awesome Media Design`, with the awesome badge on the same line.
- The first section is `## Contents`: one flat line for each `##` section. Do not list `Contributing` in it.
- Entry format: `- [Name](url) - Description.`
- The description is one short sentence. It starts with an uppercase letter and ends with a period.
- The description is objective. It does not repeat the name of the tool.
- Each entry links to the official website, and the link works. No entries without a link, no placeholders.
- Use the correct product names: Node.js, JavaScript, GitHub, macOS.
- Do not hard-wrap lines. Do not add a license section or a CI badge to the README.
- Add only tools that someone can recommend. The list is a curation, not a collection.
- Keep the CC0 license, the `main` branch, and the topics `awesome` and `awesome-list`.

## Differences from the awesome rules (on purpose)

- Tools are in A to Z order under each sub-heading. The awesome rule adds new items at the bottom, which causes merge conflicts when many students edit at the same time.
- Section headings use sentence case (`## Photo and video`). The main heading stays in title case.
- The description starts with the cost when the tool has one: Free, Freemium, Paid or Open-source. Places and hardware have no cost word.
- Sections have `###` sub-headings. A sub-heading name can repeat in different sections (for example `Spaces`, `Live coding`).
- HEAD and HES-SO places go in the section that fits, with "at HEAD" or "HES-SO" in the description.
- Missing links and techniques with no tool are GitHub issues with the label `good first issue`, not README entries.

## Checks

- `awesome-lint` (pinned to 2.3.0) and `link-check` (lychee) run on each pull request and on each push to `main`.
- The ruleset "main: required checks" blocks a merge until both checks pass. Organisation admins can bypass it.
- lychee accepts 403 and 429, because some large sites block bots.
- If a site times out only from GitHub runners, add a regex for it to `.lycheeignore`.
- To run awesome-lint locally, use `npx awesome-lint@2.3.0`. It needs the `origin` remote and an upstream branch for `main`.
- Workflows from a first-time contributor wait for a maintainer to click "Approve and run". This setting is on purpose.

## Writing style

- Write in English.
- Use ASD-STE100 (Simplified Technical English) in `contributing.md`, issues and pull request text: short sentences, active voice, one instruction in each sentence.

## Commits

- Do not add `Co-Authored-By` lines or other AI attribution to commits or pull requests. This keeps the history easy to read for the students.
- Write a short subject in the imperative mood, for example `Add Audacity` or `Fix the link for Wix`.
