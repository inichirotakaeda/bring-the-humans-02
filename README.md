# Bring the Humans Again — A Getting-Started Guide to Your First make.fun Bounty

> **For the make.fun bounty `bring-the-humans-02` ($1,000 · closes 21 Nov 2026, 17:30 WIB).**
> A plain-language guide for someone who has never entered a make.fun bounty
> before. Free to follow: no fees, no wallet, no paid tools.

---

## 1. What make.fun is

[make.fun](https://make.fun) runs coding bounties. Each bounty posts a brief
("build X"), a prize pool, and a deadline. You build the thing in your own
GitHub repository, record your builder session, and submit the repo plus a
transcript bundle. Judges review the work; prizes are split across ranked
places (for example, 1st $400, 2nd $200, 3rd $120, 4th–10th $40 each in a
$1,000 pool).

You do **not** need to be a professional developer. Bounties range from tiny
(a chess engine in 4 KB) to large (a full 3D game). Pick one that matches
what you can actually finish before the deadline.

## 2. The five rules that decide whether your entry counts

Learn these first — they are the most common reasons a good entry is rejected.

1. **One account per person.** One make.fun account, one GitHub account,
   both yours. Never borrow or share an account.
2. **Your own repo, your own code.** Every round is a **new repo with new
   code**. Re-submitting an old repo, or forking someone else's entry and
   changing a little, does not count. Aim for at least **30% authorship** of
   what you submit — the work must be visibly yours.
3. **Record before you build.** Start the session recorder **before** you
   open your editor or AI builder. The recording is the proof that you built
   it. If you start building first and record later, that work is
   unverifiable.
4. **Stop recording, then wait, then finish.** When the work is done, turn
   the recorder **off** and wait about **60 seconds** before you press
   finish/seal. Sealing too fast can cut off the end of the recording.
5. **Free only.** A legitimate bounty never asks you to pay a fee, connect a
   wallet, or sign a transaction. If a page asks for any of those, stop —
   that is not part of make.fun.

## 3. Setup (do this once, before your first bounty)

### 3.1 A GitHub account

1. Create a GitHub account with **your own** email address.
2. Pick a username you are happy to keep — it will be on every entry you
   ever submit.
3. Turn on two-factor authentication.
4. Create a **new, empty repository** for the bounty you are entering.
   Name it after the bounty (for example `bring-the-humans-02`).

### 3.2 Connect GitHub to make.fun

1. Sign in at [make.fun](https://make.fun).
2. Connect the **same** GitHub account you just created. The repo you
   submit must belong to this connected account — a repo under any other
   account will not be accepted.
3. Open the bounty page and read the brief twice: the deliverable, the
   deadline (including timezone — make.fun deadlines here are in WIB,
   UTC+7), and any required files.

### 3.3 Your tools

- A code editor you already know (VS Code is fine).
- A terminal. Most bounties run with plain commands: `node`, `python3`,
  `git`.
- The AI builder of your choice, if you use one — but see rule 2: the work
  still has to be yours, and you must be able to explain every file you
  submit.

## 4. Picking your first bounty

| Ask yourself | Good first pick | Bad first pick |
|---|---|---|
| Can I finish it before the deadline? | Yes, with a day to spare | Only if nothing goes wrong |
| Do I understand the brief in one read? | Yes | No — and the brief is long |
| Is the deliverable one clear thing? | A single script, a small game, a guide | A whole platform |
| Does it need a skill I don't have? | No, or one small thing I can learn | Three new frameworks |

Start small. A finished small entry beats an unfinished ambitious one —
and a finished entry teaches you the whole submission flow for next time.

## 5. Building: a workflow that works

1. **Read the brief again and write a one-paragraph plan.** What is the
   deliverable, what does "done" look like, what will you test?
2. **Start the recorder first** (rule 3). Then open the editor.
3. **Build the smallest working version first.** A chess engine that plays
   one legal move beats a half-written engine with a fancy UI. A game with
   one level that runs beats five levels that crash.
4. **Test as you go.** Run the program after every meaningful change. Keep
   a short note of what you tested and what passed — it becomes your
   transcript notes later.
5. **Keep the repo clean.** Only the files the entry needs: source code, a
   README, a LICENSE, and screenshots. No `node_modules`, no API keys, no
   passwords, no personal data.
6. **Write the README while you build, not after.** See section 6.

## 6. The README: what judges actually read

Your README is the entry's front door. A good one has:

- **One line** saying what it is and which bounty it is for.
- **How to run it** — exact commands, copied from a terminal where they
  worked. No "should work" — only commands you ran.
- **What it does** — the features, in plain words.
- **How it works** — a short design note (a paragraph, not an essay).
- **How you tested it** — what you ran, what passed.
- **Known limits** — what it does not do yet. Honest limits build trust;
  hidden ones get found anyway.

Example (from a real $500 entry, a 4 KB chess engine):

```text
# Chess engine 4KB — make.fun bounty ($500)
- `main.py` — 4,082 bytes (limit 4,096). Full UCI engine, Python stdlib only.
- Run: `python3 main.py`, then send UCI commands (`uci`, `isready`, `go`).
- Design: 0x88 board + vertical flip so the side to move is always "White".
- Tests: perft, self-play and UCI protocol tests all pass.
```

## 7. The submission bundle

For `bring-the-humans-02` the entry is a **guide**, so the bundle is:

| File | What it is |
|---|---|
| `README.md` | This guide |
| `LICENSE` | MIT License (see below) |
| `screenshot-*.jpg` | A screenshot of the guide, so judges can see it at a glance |
| Transcript bundle | The transcript of your recorded builder session |

For a **code** bounty the bundle is the same shape: repo + README +
LICENSE + 3–4 screenshots + transcript bundle. Check the bounty page —
some bounties ask for a live recording instead of (or as well as) a
transcript. **This bounty does not: no live recording is required.**

### LICENSE

Use the MIT License. It is one file, it is free, and it is what make.fun
entries normally carry. Put your own name and the year in the copyright
line:

```text
MIT License

Copyright (c) 2026 <Your Name>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 8. Submitting

1. Push the finished repo to GitHub. Check on github.com that the files
   you expect are actually there.
2. **Stop the recorder, wait ~60 seconds, then finish/seal** (rule 4).
3. On the bounty page, submit the repo link plus the transcript bundle.
4. **Tell someone before you submit** if you are working as a team —
   submitting is the point of no return for that round.
5. After submitting, do not edit the repo until judging is over. If the
   bounty allows resubmission, the page will say so.

## 9. After you submit

- Results usually take a few days. You will be notified on make.fun.
- If you win, the prize goes to the wallet/account you registered — make
  sure that is set up **before** the bounty closes, not after.
- Whether you win or not, keep the repo. It is your portfolio, and the
  next bounty starts from what you learned here, not from zero.

## 10. Checklist (copy this for every bounty)

- [ ] Brief read twice; deadline and timezone noted
- [ ] New repo under my own connected GitHub account
- [ ] Recorder started **before** building
- [ ] Smallest working version runs
- [ ] README written (run commands tested by copy-paste)
- [ ] LICENSE (MIT) in the repo
- [ ] Screenshots taken (3–4, each under the size limit on the bounty page)
- [ ] Transcript bundle saved
- [ ] Recorder off, waited ~60 s, then finished/sealed
- [ ] Submitted before the deadline — and told my teammate first

## 11. FAQ

**Do I need to pay anything?**
No. Entry is free. If anything asks for money, a wallet connection, or a
signature, stop.

**Can I use AI to build my entry?**
Yes — most entrants do. But the entry must be yours: new repo, new code,
at least ~30% your authorship, and you must be able to explain it. The
recording proves you built it; AI output you cannot explain is a weak entry.

**What if I miss the deadline?**
The round closes when it closes. Submit early — an entry submitted a day
early beats a perfect entry submitted a minute late.

**My recording didn't start before I built. What now?**
That session's work is unverifiable. Start a new recorded session, rebuild
(or continue building) inside it, and submit the recorded work.

**Can I enter the same bounty twice?**
Each round is a fresh entry: new repo, new code. Read the bounty page for
the round you are entering — rules can change between rounds.

**Where does the prize go?**
To the payout destination on your make.fun account. Set it up before the
bounty closes.

---

*Written for first-time entrants. Built from real entries: a 4 KB chess
engine ($500 bounty, closes 25 Nov 2026) and VOLTLINE, a three.js tactical
FPS ($1,000 bounty, deadline 24 Nov 2026). Good luck — start recording,
then start building.*
