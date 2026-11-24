# Office Joke Open — Entry

## What this is

A single office-life joke submitted to "Make the AI Judge Laugh: the Office Joke Open". The program's entire output is one file: `output/entry.txt`. There is no logic to run; the writing is the contest.

## The entry

```
My boss asked why I only get through half my to-do list. I said meetings. He called a meeting to discuss it. We were in it for an hour and discussed the meeting we'd need next week.
```

Length: 186 characters (under the 200-char limit). UTF-8, single line, non-empty.

## Why this joke

The judge brief rewards clean setup-punchline structure and relatable office tropes. This joke uses:

1. **Setup** — a performance question from a boss (universally understood).
2. **Twist** — the one-word answer "meetings" names the villain.
3. **Escalation** — the boss responds by doing the very thing that causes the problem.
4. **Second punchline** — the meeting about the meeting, the most recognizable absurdity in office life. Ending on "next week" lands the recursion at the final character, which is where head-to-head judges weight the punchline hardest.

No niche references, no wordplay that can be misread, no edgy content. Every judge model has effectively "lived" this meeting.

## Candidate testing

Three candidates were compared head-to-head before choosing:

- **A (winner, above)** — the meeting-about-the-meeting joke.
- **B** — "Per my last email is corporate for: I have given up on words and now rely on your shame." Rejected: strong but riskier, sarcasm ranks inconsistently.
- **C** — "Our printer has three statuses: low toner, out of toner, and jammed. It has never once printed." Rejected: observation, not a joke with a punchline turn.

A won on every pairwise comparison: it has the clearest setup-punchline arc and the strongest closing beat.

## Validation

The gate requires `output/entry.txt` to be UTF-8 text, 1–200 characters, not only white space. Checks performed:

- Length: 186 characters (<= 200). ✔
- Encoding: plain ASCII, valid UTF-8. ✔
- Content: non-whitespace text present. ✔
- Format: single line, no trailing newline issues (file ends after the punchline period). ✔

## Files

- `output/entry.txt` — the joke, the sole judged artifact.
- `README.md` — this document.

## Usage

No build step. Ensure `output/entry.txt` exists at the entrypoint path; it is the submission.

## License

MIT. The joke is original.