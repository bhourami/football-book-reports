# ⚽ Football Book — Results

The published results of a personal, real-money betting research project.
Two AI analysts (Claude and Codex) pick Premier League singles independently,
blind to each other until after they've both committed, then debate it out.
Three scorecards run side by side — Claude solo, Codex solo, and whatever the
two of them agree on after arguing — so it's possible to tell whether the
arguing is actually worth anything.

**This is not tipping and nothing here is betting advice.** See
[Notice](#notice) below before reading anything here as a recommendation.

## How a pick gets made

1. **Kick-off, not full time.** Every question here settles in ninety
   minutes. No waiting on a slow-moving story.
2. **Blind first.** Claude and Codex each write down their pick — team,
   market, price, stake — before either has seen the other's. No peeking,
   no reacting to a pick that was never really independent.
3. **Then the debate.** They challenge each other's reasoning until neither
   has anything left to add or change.
4. **Only a real disagreement stays a disagreement.** If they land on the
   same pick, that's the "conclusion" book's bet. If they don't agree, the
   conclusion book sits it out — no averaging, no coin flip.
5. **No news, no bet.** If team news isn't confirmed before kick-off, that
   fixture is a pass, full stop — not a smaller bet, not a guess.

## What's tracked, and why it's not just profit and loss

Twenty or thirty bets isn't enough to prove a betting strategy works or
doesn't — a perfectly good process can lose money over a small sample, and a
lucky one can win. So alongside the running scoreline, every bet is checked
against **closing line value**: did the price obtained beat the price the
market settled on by kick-off? That's the harder number to fake, and the one
that means something well before the bank does.

- `reports/` — one file per published update: current standings across all
  three books, and the settled bet-by-bet history.
- Declined picks are published too, not just the ones that were taken — a
  book that's ahead because of what it *refused* to bet on is exactly the
  kind of thing that's invisible unless it's written down.

## Numbers so far

The season's already under way, with fixtures this week and every week —
this pipeline just hasn't placed its first bet yet. See
`reports/current-status.md` for why, and what's left to set before it does.

## Asking for something

Open an issue using one of the templates:

- **Fixture check** — look at one specific upcoming match.
- **Ledger refresh** — regenerate the published standings from the private
  ledger (mechanical only; doesn't call either analyst or change a pick).

A request here doesn't create a bet, change a stake, or skip any rule in the
methodology. The full rule set, the ledger, and the debate transcripts stay
in the private working repo; this one holds only the finished, settled
results.

---

## Notice

**Not betting advice.** Nothing here is a recommendation, inducement or
invitation to place a wager. This is the output of a personal research
project, published so the author's own tools can read it — it takes no
account of anyone else's circumstances or risk tolerance and isn't suitable
as a basis for anyone else's decision.

**Real money, owner-placed only.** The stakes and results here are real, not
notional. Every bet is placed by the account owner himself, by hand, at
whatever price he actually gets. Nothing in this project, or anything
publishing to it, ever holds or uses a bookmaker account's credentials.

**No regulated activity.** The author isn't authorised or regulated by the
Gambling Commission or any other regulator, and isn't a tipster or betting
adviser acting in any professional capacity. Nothing here is a financial
promotion, a gambling inducement, or an offer to anyone else.

**No warranty.** This may be incomplete, out of date, or simply wrong. It's
provided as-is, with no duty of care to any reader. If you're reading this
and you're not the author: don't rely on it, and don't use it as a basis for
placing a bet of your own.

**If gambling stops being fun** — chasing losses, spending more than
planned, or just not enjoying it any more — begin.gambleaware.org or the
National Gambling Helpline (0808 8020 133, free, 24/7) are independent of
this project and of any bookmaker.

**Third-party material.** Fixture data, prices and statistics referenced
here remain the property of their respective providers, cited for
verification only.
