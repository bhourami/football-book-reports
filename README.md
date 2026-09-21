# ⚽ Football Book

Two AI analysts (Claude, Codex) price Premier League matches
independently, then argue. Public in full — losses, errors and
corrections included. Not betting advice — see [Notice](NOTICE.md).
How it works: [Process](PROCESS.md).

> **Reset, 21 September 2026.** The staking era is closed and archived.
> It finished **£35.09 up** over 15 bets, and stopped anyway. Everything
> below is the new regime: **no money is staked**, and the scoreboard is
> no longer profit.

## The scoreboard is now closing line value

| | |
|---|---|
| Selections recorded | **0** |
| Scored | 0 |
| Median CLV | — |
| Decision point | **60 selections** |

Nothing has been recorded yet. Collection starts at Matchweek 6,
10–12 October.

### What that means

When a market closes, its price is the most accurate estimate anyone
ever produces of what was actually going to happen — every bit of team
news and every pound of informed money has gone in. Strip the
bookmaker's margin out of that closing price and you have the best
available measure of the truth.

Closing line value is the gap between the price we called and that
number. It is not a proxy for having an edge. **It is the edge**,
expressed as expected value:

> **EV = fair closing probability × the price we called − 1**

A call with positive CLV makes money in the long run whether or not it
wins. A call with negative CLV loses money in the long run however often
it wins. Results are still recorded here, as facts — they are just not
the score.

### Why not profit

Because profit can't answer the question at this scale. Here are three
real bets from the old era, measured against margin-removed closing
prices:

| Bet | Called at | Fair closing price | EV per £10 |
|---|---|---|---|
| Coventry v Brighton, Draw | 3.70 | 4.00 | **−£0.75** |
| Leeds v Newcastle, Newcastle | 2.90 | 3.16 | **−£0.81** |
| Man Utd v Man City, Man City | 2.15 | 2.33 | **−£0.78** |

Every one expected to lose about 78p per £10 the moment it was placed.
One of them won.

Look at how close those three are. That is not luck — it is a stable
property of the method, visible in **three** bets. The profit over
fifteen bets was **+£35** and told us nothing at all. CLV converges in
tens because it measures the price; profit needs hundreds because it
measures coin flips.

**The decision rule, fixed in advance:** after 60 selections, if median
CLV is at or below zero, this method cannot price football better than
the market and the project stops looking for edge. No extension, and no
early stop because a run of results looks good.

## Two other things changed

**Prices are now referenced to a betting exchange, not a bookmaker.**
A bookmaker builds 5–7% margin into the quoted price; an exchange
charges commission on net winnings only. The same three calls were worth
better prices at Betfair — 3.90 instead of 3.70, 3.15 instead of 2.90,
2.30 instead of 2.15.

> **Corrected by Codex, 21 September 2026.** This section first said the
> exchange takes the method "to roughly break-even". **That was wrong.**
> Commission applies to net winnings, so the effective price is
> `1 + (odds − 1) × (1 − commission)`, applied *before* computing EV.
> Recomputed:
>
> | | Mean EV per bet |
> |---|---|
> | Bookmaker | −7.80% |
> | Exchange at 2% commission | **−2.68%** |
> | Exchange at 5% commission | **−4.64%** |
>
> The exchange recovers about 5 points and **stays negative**. It makes
> the method lose less. It does not make it break even.
>
> This makes the problem harder, not easier: breaking even on the
> exchange now requires demonstrated edge of at least **2.7 percentage
> points** against the closing line, not zero.

Codex predicted, without having seen Claude's position, that its likely
error would be *"believing exchange pricing plus richer AI analysis
closes the remaining gap"* — and then found exactly that error. Both
answers and the reconciliation are in the
[working repo](https://github.com/bhourami/football-book/tree/main/collaboration/debates/profitability-2026-09-21).

**The competition stays the Premier League**, which was checked rather
than assumed. Median bookmaker margin across full fixture lists:

| League | Margin |
|---|---|
| Premier League | **7.34%** |
| Championship | 8.28% |
| League Two | 9.28% |

Lower divisions are *more* expensive, not less. They are priced less
accurately, but the bookmaker charges a wider margin precisely because
it is less confident — so you would need to be about 2pp better than the
market just to stand still.

## The era that just closed

| Book | Real money? | Final | Net | Bets |
|---|---|---|---|---|
| Codex solo | Yes | £251.09 | +£51.09 | 7 |
| Conclusion (debated) | Yes | £194.00 | −£6.00 | 7 |
| Cross-book accumulators | Yes | own pot | −£10.00 | 1 |
| Claude solo | Never staked | — | +£4.25 paper | 6 |
| **Combined** | | | **+£35.09** | **15** |

It closed while **ahead**, on a rule written when the books were flat.
That is the only circumstance in which a pre-commitment costs anything
to honour, and therefore the only one in which honouring it proves
anything.

The reason: a model walked forward over **1,180 matches** beat the
closing line about **50%** of the time — a coin flip — while selecting
**72.5%** of available markets. A method that finds edge in seven
matches out of ten is disagreeing with the market at random.

**What it actually produced** was a record of how a confident method
manufactures edge that isn't there. Three numbers in that era were
*typed rather than derived* — a scoreline from a web fetch, the running
totals, and the single positive CLV figure ever published here — and all
three were wrong in the flattering direction. Every one is corrected in
place, with the original wording shown.

- [Matchweek 5](reports/matchweek-5.md) — Codex +£51.09, conclusion −£6.00, BTTS finished 8-8
- [Matchweek 4](reports/matchweek-4.md) — conclusion −£14, and a corrected CLV claim
