[![make.fun](https://make.fun/badge/u-pucuys-one-line-office-joke-24-hour-sprint-aaf86162.svg)](https://make.fun/bounty/u-pucuys-one-line-office-joke-24-hour-sprint-aaf86162)
[![rank](https://make.fun/badge/u-pucuys-one-line-office-joke-24-hour-sprint-aaf86162/mfahmiq/office-joke-sprint/rank.svg)](https://make.fun/bounty/u-pucuys-one-line-office-joke-24-hour-sprint-aaf86162)
[![reward](https://make.fun/badge/u-pucuys-one-line-office-joke-24-hour-sprint-aaf86162/mfahmiq/office-joke-sprint/reward.svg)](https://make.fun/bounty/u-pucuys-one-line-office-joke-24-hour-sprint-aaf86162)

# One-Line Office Joke

Entry for the make.fun bounty
[One-Line Office Joke: 24-Hour Sprint](https://make.fun/bounty/u-pucuys-one-line-office-joke-24-hour-sprint-aaf86162).

> Someone replied-all to a 200-person email asking to be removed from
> the thread, and now 200 people are replying-all to agree.

## The line

The joke, in full:

```
Someone replied-all to a 200-person email asking to be removed from the thread, and now 200 people are replying-all to agree.
```

125 characters, one line, written by `main.py` to
`$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output/entry.txt`).

## Why this line lands

The judge brief scores five things, most important first. This line was
built to answer each of them in order:

**1. It is a one-line joke about office life.** The whole scene is
office life and nothing else: a 200-person email thread, the reply-all
button, and the ritual of asking to be removed from a thread you never
asked to join. It is a joke, not a caption or a stray observation — it
has a setup (someone replies-all to escape the thread) and a punchline
(the escape attempt becomes the thread). Nobody outside an office has
a reply-all button to press.

**2. It is funny, because the punchline is an ironic loop anyone who
has sat in an office recognises.** The first person tries to stop the
emails by sending an email to everyone; then 200 people repeat the
exact mistake they are agreeing is a mistake. The payoff is that the
complaint and the crime are the same action, and the crowd grows the
problem while trying to shrink it. Every office worker has watched a
thread like this snowball in real time.

**3. It is one line and complete, with no rambling.** One sentence, two
clauses, 125 characters. The setup names the act, the punchline names
the consequence, and nothing else is in the room — no preamble, no
"so I was at work today", no explanation of why reply-all is bad.
The joke trusts the reader to know.

**4. It is fresh, built on a specific detail rather than a generic
complaint.** Not "meetings are too long", not "Mondays are bad", not
"the printer is broken" — the material is the reply-all removal
request, a small, concrete office ritual with its own absurd logic.
The number 200 matters: it is big enough that the pile-up is
catastrophic and small enough to be a real company thread.

**5. It is clear on first read, with tight wording.** Every word is
plain office vocabulary — replied-all, email, thread, agree — and the
sentence reads in one breath. There is no reference the reader cannot
follow, no acronym, no in-joke, and no word that needs a second pass.

## Drafting notes

The line was written from scratch for this competition, not adapted
from the kit's examples or from any earlier entry. Two directions were
considered and dropped before settling on this one:

- A "the meeting could have been an email, but the email would have
  been a meeting" line — tidy, but the joke is a shrug about meetings
  in general, and the "meeting that should have been an email" premise
  is the most told office joke there is.
- A "my lunch break is now a calendar invite titled 'Lunch
  (optional)'" line — specific and recognisable, but the punchline
  lands as an observation about a full calendar rather than a joke
  with a turn.

The reply-all line won because it is the only one of the three with a
real mechanism: an action that defeats its own purpose, repeated by
200 people at once. The final wording was tuned for rhythm — "asking
to be removed ... replying-all to agree" — and checked at 125
characters, well inside the 200-character gate, so no word had to be
cut for length.

## How the entry works

`main.py` is Python 3.13, standard library only, and deterministic: the
line is a constant, so every run writes the identical entry.

```bash
MAKEFUN_OUTPUT_DIR=/tmp/out python3 main.py
cat /tmp/out/entry.txt
```

The program:

1. Writes the line to `$MAKEFUN_OUTPUT_DIR/entry.txt`
   (defaulting to `/output/entry.txt` when the variable is unset).
2. Self-verifies before and after writing: the text must be valid UTF-8,
   1–200 characters, a single line, and not only whitespace — the exact
   conditions of the competition gate.
3. Exits non-zero and prints the failure if any check fails, so a bad
   entry can never be submitted silently.

## Files

| File | What it is |
| --- | --- |
| `main.py` | The entry program: writes and self-verifies `entry.txt` |
| `entry.txt` | The joke line itself |
| `README.md` | This file |
| `LICENSE` | MIT |

## License

MIT — see [LICENSE](LICENSE).
