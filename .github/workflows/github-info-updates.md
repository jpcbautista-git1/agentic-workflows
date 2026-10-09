---
on:
  workflow_dispatch:
permissions:
  contents: read
engine: copilot
network:
  allowed:
    - defaults
    - github.blog
tools:
  web-fetch:
safe-outputs:
  create-pull-request:
    title-prefix: "[github-info] "
    draft: false
---

# Update Mona's GitHub Info website

## Purpose
Keep Mona's GitHub Info website current with relevant GitHub news.

## Sources to consult
1. Mona's notes: `notes/mona-notes.md` (her interests and priorities).
2. GitHub Blog: https://github.blog/
3. GitHub Changelog: https://github.blog/changelog/

## Files you may modify
- Only files in `site/` (the website). Do not modify workflows, notes, or any other files.

## Steps
1. Read Mona's notes.
2. Review posts from the last 14 days on the Blog and Changelog.
3. Pick the 3–5 updates most relevant to Mona's notes.
4. Draft concise website updates: a title, a 1–2 sentence summary, and a source link for each.
5. Open a pull request with the changes.

## Pull request format
- **Summary** of what changed.
- **Sources used**: a list of every Blog or Changelog URL, plus a note that Mona's notes were read.
- **Why each update is relevant** to Mona.

## Review process
A human must review and approve this pull request before it is merged. Never merge automatically.