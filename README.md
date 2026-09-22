# Raider Clavier

**Type French on a US keyboard.** A typing tutor for Regis Jesuit French students, covering
the two Windows layouts a student here might actually be running.

**Live:** https://rjedtech.github.io/Raider-Clavier/

One file. No server, no accounts, no build step. Everything a student types stays in their
browser.

## Two layouts, one tool

| | US-International *(default)* | French (France) AZERTY |
|---|---|---|
| Letters | stay where they are printed | A↔Q, Z↔W, M moves beside L |
| Digits | normal | need Shift |
| é | `'` then `e` | its own key (printed `2`) |
| è à ù | `` ` `` then the vowel | their own keys (`7`, `0`, `'`) |
| ç | `'` then `c` | its own key (printed `9`) |
| ê â î ô û | `Shift`+`6` then the vowel | the key printed `[` then the vowel |
| ë ï ü | `Shift`+`'` then the vowel | `Shift` + the key printed `[` |
| **É and Ç** | `'` then `Shift`+letter | **not possible** — no acute or cedilla key exists |
| « » | `AltGr`+`[` and `AltGr`+`]` | not on this layout |

Switch layouts at the top of the page. Every keycap, hint, cheat sheet and setup guide
rebuilds; the drill you are in carries on with the same words.

**US-International is the default** because it is the school standard. LockDown Browser is
deliberately restricted and the Canvas special-characters ribbon can vanish mid-quiz, so
accents need to come from the keyboard itself. It is also the only one of the two that can
type capital accented letters at all.

Mappings were taken from the Windows layout drivers themselves (`kbdfr.dll`, `kbdusx.dll`),
not from memory.

## What's in it

- **Layout check** — one keypress that tells a student whether they are actually on the
  layout they think they are. Catches the failure that otherwise makes every drill feel broken.
- **Eight drills** — é, è à, ç ù, circumflex, tréma, the rest of the keyboard, full
  sentences, and accent practice (the word appears stripped of accents; the student supplies them).
- **Sprint** — 30 s / 60 s / 2 min. Accented characters score 25 against an ordinary letter's
  10, so the scoring rewards exactly what the class is about.
- **My progress** — personal bests, weak keys, badges, and a report to attach to a Canvas
  assignment.
- **Class leaderboard** — for the teacher. There is no server, so students paste a short
  score code into Canvas or Teams and the teacher pastes the pile in here. Edited codes are
  shown but flagged, and a valid code always outranks a tampered one.
- **Shortcut sheet** — every French character on the layout you picked, including the ones
  neither layout can produce (`œ`) and how to get them anyway.

## For teachers

Paste your own word or sentence list under **Practice → Teacher**. "Copy student link" packs
the list into the URL, so students open straight into it — nothing to type, no accounts.

A note on the leaderboard: typing speed is a motor skill with an objective number, which is
the friendliest case for ranking a class. A permanent public ranking is still the weakest
form of gamification. Consider running it as a single-round arcade score that resets, or
ranking by each student's gain over their own first sprint. Personal bests are already
tracked privately either way.

## Privacy

No network calls, no accounts, no analytics beyond an anonymous page count. Progress lives in
`localStorage` under `rjclavier_v1` on the student's own machine.

---

Regis Jesuit · Educational Technology
