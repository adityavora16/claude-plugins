# Claude Code plugins by Aditya Vora

**Two free Claude Code plugins, installed with two commands each: shorter answers, and big jobs split into parallel sessions.**

| Plugin | What it does | Repo |
|---|---|---|
| `terse` | Claude answers in the first sentence and stops when the answer is complete, with the AI writing tells stripped from the words that stay. | [adityavora16/terse](https://github.com/adityavora16/terse) |
| `session-board-lite` | Splits one big job into Claude Code sessions you can run in parallel and builds a local board with one paste-ready prompt per session. | [adityavora16/session-board-lite](https://github.com/adityavora16/session-board-lite) |

## Install

Needs Claude Code 2.1.116 or newer.

```bash
claude plugin marketplace add adityavora16/claude-plugins
claude plugin install terse@adityavora
claude plugin install session-board-lite@adityavora
```

Inside a session, `/plugin marketplace add adityavora16/claude-plugins` and `/plugin install
<name>@adityavora` do the same, and `/plugin` lets you browse the list. The marketplace's name is
`adityavora`; the repo is `adityavora16/claude-plugins`.

## Sample

Asked "Does `Array.prototype.sort` sort numbers numerically by default?", Claude with Terse replies:

> No. It sorts as strings, so `[10, 9, 1]` becomes `[1, 10, 9]`. Pass `(a, b) => a - b`.

Session Board Lite builds a board like this from a one-line job description:

![A Session Board Lite board for an invented three-session job](https://raw.githubusercontent.com/adityavora16/session-board-lite/main/screenshot/board-lite.png)

## More for editors

Paid Claude Code skills from the same author:

- [Editor's Brain](https://adityavora.gumroad.com/l/editors-brain?utm_source=github&utm_medium=readme&utm_campaign=useu-q4): the planning half of editing, done to a method, from one script.
- [Session Board](https://adityavora.gumroad.com/l/session-board?utm_source=github&utm_medium=readme&utm_campaign=useu-q4): a paste-ready prompt for every session, on one board, kept current as sessions report back.
- [AE Script Builder](https://adityavora.gumroad.com/l/ae-script-builder?utm_source=github&utm_medium=readme&utm_campaign=useu-q4): scripted After Effects comps, checked before you press Run.
- [Chart Shorts Kit](https://adityavora.gumroad.com/l/chart-shorts-kit?utm_source=github&utm_medium=readme&utm_campaign=useu-q4): numbers in, a finished 38-second chart Short out. No After Effects.

## Licence

The marketplace file is MIT. Each plugin carries its own licence in its repo.
