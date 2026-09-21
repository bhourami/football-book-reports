# ⚽ Football Book — Results

Real-money Premier League picks from two independent analysts (Claude,
Codex) plus whatever they agree on after debating. Not betting advice —
see [Notice](NOTICE.md). How picks are actually made: [Process](PROCESS.md).

## Running total

Carried across every gameweek. Both real-money books started at £200.

| Book | Real money? | Bank | Net so far | Bets settled |
|---|---|---|---|---|
| Codex solo | **Yes — actual stakes** | **£251.09** | **+£51.09** | 7 |
| Conclusion (debated) | **Yes — actual stakes** | **£194.00** | **−£6.00** | 7 |
| Claude solo | Tracked only, never staked | £204.25 if funded | +£4.25 | 6 on paper |
| Cross-book accumulators | **Yes — actual stakes** | own pot | **−£10.00** | 1 |

**Combined real money across all three pots: +£35.09.**

> **Correction, 21 September 2026.** This line first read "−£10.00",
> which was the accumulator pot's figure mistaken for the combined one.
> The real combined position is **+£35.09**. It is now computed by
> `scripts/totals.py` rather than typed, the same fix applied to the
> per-book figures a day earlier.

Codex's book is £51 up after a very good Sunday. That is 7 bets, and it
should not be read as skill — see below.

## Nothing is pending

Matchweek 5 is settled and filed. **No picks are live, and none are
scheduled.** The next Premier League fixtures are Matchweek 6 on 10–12
October.

## Why there are no new picks

In September the forecasting model behind every pick on this page was
fitted properly and tested the honest way — walked forward over **1,180
matches**, never seeing a result before predicting it.

It found **no edge over the closing line at any threshold.** It beat the
closing price about 50% of the time, which is a coin flip. Under the
live selection rule it would have staked £8,560 and lost £787.30, a
−9.2% return. It selected **72.5% of available markets** — a method that
finds edge in seven matches out of ten is disagreeing with the market at
random, not finding value.

**Both analysts independently recommended stopping staking under that
rule.** That decision belongs to the owner and is still open.

This page is kept public in full, losses and corrections included,
because a betting record that only appears when it is winning is not a
record.

## The BTTS market is paused

Flagged by the owner on 19 September: every both-teams-to-score pick
across an entire gameweek came back "No". Checked rather than defended,
and the pattern was real — each analyst's own "No" probability sat above
the market's fair "No" probability, every single time. Not independent
value-finds; a systematic skew.

A fitted model then confirmed it is structural: predicted
both-teams-to-score at 54.3% against a realised 58.1%, and 18.5
percentage points wrong in exactly the bucket where "No" looks most
tempting.

All staked BTTS picks have now settled. The finished record:

| | |
|---|---|
| Settled BTTS selections | 16 |
| Won | 8 |
| Lost | 8 |
| Of which "No" | **15 of 16** |
| Net | +£26.59 |

**Eight and eight** — an exact coin flip, positive only because the
winners came at longer prices than the losers. Man City 5-3 Sunderland,
eight goals, is what it looks like when that lands badly on real money.

The pause was questioned after three BTTS wins in a row over the
weekend. Three wins is not evidence against a 1,180-match measurement,
and *winning* is not the same as being *correctly priced*: a bet landing
half the time at around 2.00 is break-even, not edged. **The pause
stands.**

## What happens next

A [pre-registered experiment](https://github.com/bhourami/football-book/blob/main/spec/experiment-02-price-comparison.md)
that uses **no forecasting model at all**, and no opinion about who will
win. It asks one narrow question: does the bookmaker actually used ever
offer a price better than the wider market's margin-adjusted consensus,
and does it last long enough to place by hand?

The thresholds, the decision rule and the stopping rule were all written
down **before any data was collected**, so they cannot be adjusted later
to make a result look better. Returning **nothing** is the expected
outcome, and all four conditions must pass to justify any real-money
trial. If one fails, this project stops looking for edge in retail
football betting.

**No money is staked on anything arising from it.** Collection starts at
Matchweek 6.

## Past weeks

- [Matchweek 5](reports/matchweek-5.md) — Codex solo **+£51.09**,
  conclusion book **−£6.00**, BTTS finished level at 8-8
- [Matchweek 4](reports/matchweek-4.md) — conclusion book **−£14**,
  Codex solo +£8.75 on paper
