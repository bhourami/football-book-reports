# ⚽ Football Book — Results

Real-money Premier League picks from two independent analysts (Claude,
Codex) plus whatever they agree on after debating. Not betting advice —
see [Notice](NOTICE.md). How picks are actually made: [Process](PROCESS.md).

> **BTTS market paused, 19 September 2026.** Every BTTS "No" pick this
> gameweek (9 of 9 for Codex, 2 of 2 for Claude) shared the same
> problem: the analyst's own "No" probability was higher than the
> market's fair "No" probability, every single time — not independent
> value-finds, a systematic skew in how both methods estimate expected
> goals. No new BTTS selection until that's fixed with real scoring
> data instead of a qualitative guess. Pending BTTS picks below are
> already staked and settle as normal, but shouldn't be read as
> verified edges.

## Running total

| Book | Real money? | Bank (from £200) | Settled | Still live |
|---|---|---|---|---|
| Conclusion (debated) | **Yes — actual stakes** | £194.00 | **−£6.00** over 7 bets | — |
| Codex solo | **Yes — actual stakes** | £251.09 | **+£51.09** over 7 bets | — |
| Claude solo | Tracked only, never staked | £204.25 if funded | +£4.25 on paper | — |
| Cross-book accumulators | **Yes — actual stakes** | n/a, own pot | **−£10.00** (dead — BTTS No leg lost) | — |

**Correction, 20 September 2026:** this table previously described the
Codex book as "tracked only, not staked". That was wrong — it has had
real money through it since Matchweek 5. Its tracked-only figure was
also stale. Totals are now computed from the ledgers by
`scripts/totals.py` rather than maintained by hand, which is how the
drift happened.

**Matchweek 5 is settled.** The Codex book had a very good Sunday and
is £51 up on real money; the debated conclusion book is £6 down. Before
reading anything into that: it is 7 bets. The gap between the two books
is almost entirely four Sunday results, and a fitted model walked
forward over 1,180 matches found **no edge over the closing line at any
threshold** — which is why the honest reading of a £51 fortnight is
noise, not skill. See [Process](PROCESS.md).

Tracked figures use the price at selection time; the real-money figures
use the price actually obtained.

## Matchweek 5 — placed

### Conclusion book (Claude and Codex agreed) — placed, real money

| Fixture | Kick-off | Pick | Price obtained | Result |
|---|---|---|---|---|
| [Tottenham v Aston Villa](reports/matches/2026-09-19-TOT-AVL.md) | Sat 19 Sep, 12:30 | Villa win | 3.80 | **Won** (+£28) |
| [Tottenham v Aston Villa](reports/matches/2026-09-19-TOT-AVL.md) | Sat 19 Sep, 12:30 | BTTS: No | 2.25 | **Lost** (-£10) |
| [Man City v Sunderland](reports/matches/2026-09-20-MCI-SUN.md) | Sun 20 Sep, 14:00 | BTTS: No | 1.70 | **Lost** (−£10) |

Tottenham 2-3 Aston Villa full time — net **+£18** on this fixture.

Also placed: a **"Bet Builder+" accumulator** (£10, combined price
1724.91/1) covering all ten markets below, conclusion and Codex-solo
mixed together. This initially broke the single-book accumulator rule
set after Matchweek 4 — the rule was amended the same day to allow
cross-book accumulators, since every leg had already independently
cleared its own book's threshold before the acca combined them.
Tracked in its own running total, not charged against either book's
bank.

**Lineup check, ~1hr before the 14:00 BST kick-offs (20 September):**
Bournemouth-Liverpool and Man City-Sunderland both confirmed with no
material team-news surprise on either side — see
[Bournemouth v Liverpool](reports/matches/2026-09-20-BOU-LIV.md) and
[Man City v Sunderland](reports/matches/2026-09-20-MCI-SUN.md) for the
full detail, including a modest favourable price drift on the Man
City-Sunderland BTTS pick (1.80 → 2.00) that raises both analysts'
edges further above threshold.

### Claude solo book — additional picks beyond the conclusion book

| Fixture | Kick-off | Pick | Price | Edge |
|---|---|---|---|---|
| [Newcastle v Hull City](reports/matches/2026-09-19-NEW-HUL.md) | Sat 19 Sep, 15:00 | Draw | 4.333 | +4.1pp |

Codex disagreed here — its own numbers don't clear the threshold on
this fixture, a genuine difference of view, not a data gap.

### Codex solo book — additional picks beyond the conclusion book

Ranked best to worst by how well they hold up against the actual
league table, not by raw edge size. Ranks 6 and 9 (both Fulham-Man Utd
markets) were dropped by the owner before placing, for sharing the
same suspect pattern (backing the clearly weaker, winless team) that
got Leeds-Palace withdrawn outright. Everything else was placed.

| Rank | Fixture | Kick-off | Pick | Price obtained | Result |
|---|---|---|---|---|---|
| 1 | [Man City v Sunderland](reports/matches/2026-09-20-MCI-SUN.md) | Sun 20 Sep, 14:00 | Man City win | 1.30 | **Won** (+£3) |
| 2 | [Nottingham Forest v Coventry](reports/matches/2026-09-19-NFO-COV.md) | Sat 19 Sep, 17:30 | BTTS: No | 1.91 | **Won** (+£9.09) |
| 3 | [Bournemouth v Liverpool](reports/matches/2026-09-20-BOU-LIV.md) | Sun 20 Sep, 14:00 | Liverpool win | 2.10 | **Won** (+£11) |
| 4 | [Bournemouth v Liverpool](reports/matches/2026-09-20-BOU-LIV.md) | Sun 20 Sep, 14:00 | BTTS: No | 2.70 | **Won** (+£17) |
| 5 | [Everton v Ipswich](reports/matches/2026-09-19-EVE-IPS.md) | Sat 19 Sep, 15:00 | BTTS: No | 2.05 | **Won** (+£10.50) |
| 6 | [~~Fulham v Man Utd, BTTS: No~~](reports/matches/2026-09-20-FUL-MUN.md) | Sun 20 Sep, 16:30 | *dropped before placing* | — | — |
| 7 | [Leeds v Crystal Palace](reports/matches/2026-09-20-LEE-CRY.md) | Sun 20 Sep, 14:00 | BTTS: No | 2.05 | **Won** (+£10.50) |
| 8 | [Everton v Ipswich](reports/matches/2026-09-19-EVE-IPS.md) | Sat 19 Sep, 15:00 | Ipswich win | 4.20 | **Lost** (-£10) |
| 9 | [~~Fulham v Man Utd, Fulham win~~](reports/matches/2026-09-20-FUL-MUN.md) | Sun 20 Sep, 16:30 | *dropped before placing* | — | — |

**Withdrawn as confirmed reasoning errors, not just flagged:**
- Brighton v Arsenal, Brighton win + BTTS Yes — rested on "Arsenal's
  defensive crisis," the same reasoning already withdrawn from Claude's
  book this gameweek as factually wrong (Arsenal are 6-0-0 this season
  with that same absence pattern). Reinforced by the pre-kick-off
  lineup check: only Saliba was actually out, with Timber and Mosquera
  both starting — and the market had caught up too, pushing Brighton's
  win edge negative (-3.6pp) by kick-off.
- Leeds v Crystal Palace, Palace win (+22.6pp, the largest edge
  recorded anywhere in this project) — confirmed against the live
  table: Leeds are 4th and unbeaten, Palace are 16th with one win in
  four. Backing the out-of-form team at a huge edge over an unbeaten
  top-4 side is the same failure pattern as Arsenal, not a genuine find.
  Given extra scrutiny at the pre-kick-off lineup check: Crystal Palace
  are missing their first-choice striker (Mateta) and their goalkeeper
  (Henderson), on top of a suspension, and Bet365's price is completely
  unchanged. Nothing in the confirmed team news makes the case for
  Palace stronger — decline reinforced, not just repeated.

**Fulham v Man Utd (ranks 6 and 9), lineup check, ~1hr before the
16:30 BST kick-off (last fixture of the gameweek):** confirmed lineups
show no material team-news surprise for either side, and both edges
recompute identically to their original values (+5.06pp, +3.40pp),
still clearing the 3pp threshold on today's numbers — see
[Fulham v Manchester United](reports/matches/2026-09-20-FUL-MUN.md).
This doesn't reopen either pick: they were dropped for a confidence-
ranking reason unrelated to team news or edge, and that decision
stands unchanged.

**How the withdrawals turned out.** Brighton beat Arsenal 3-0. The
withdrawn Brighton win would have returned +£20; the withdrawn BTTS Yes
would have lost. The withdrawal was still correct: it was pulled because
its stated reason was false, and the result does not make that reason
true. Arsenal were 6-0-0 with that same absence pattern, and on the day
Timber and Mosquera both started. Leeds v Palace is still to play.

**And the reverse case, on the same afternoon.** Forest 0-1 Coventry
settled the BTTS No above as a winner. That pick's stated basis was
"Coventry have literally 0 goals in 4 league games — the strongest
empirical anchor of any surviving pick". Coventry scored, away, and won.
The bet landed only because *Forest* failed to score, which formed no
part of the reasoning. The bet won and its premise was refuted in the
same ninety minutes.

Together these two are the clearest illustration this project has
produced of why outcome and decision quality are recorded separately
here: one correct decision that lost money, one flawed decision that
made money, in the same afternoon.

Nine selections here across two gameweeks is still meaningful volume
for a 20-bet book — a pattern worth watching, not yet a crisis.

**Matchweek 5 picks are now finalised.** Every fixture this gameweek
has either settled or had its pre-kick-off lineup check completed,
including Fulham v Man Utd, the last kick-off of the week. Results for
the still-pending fixtures (Bournemouth-Liverpool, Leeds-Palace,
Man City-Sunderland) will follow as those matches conclude, settled
against premierleague.com directly rather than a general fetch or
search summary.

## The BTTS picture, now that Matchweek 5 is settled

The BTTS market was [paused on 19 September](#) after every single pick
across a whole gameweek came back "No". Those already-staked picks have
now all settled, so here is the complete record across all three books:

| | |
|---|---|
| Settled BTTS selections | 16 |
| Won | 8 |
| Lost | 8 |
| Of which "No" | **15 of 16** |
| Net | +£26.59 |

**Eight and eight.** An exact coin flip, profitable only because the
winners happened to come at longer prices than the losers. Man City 5-3
Sunderland — eight goals — is what that looks like when it goes wrong on
real money.

This matters because the pause was questioned after three BTTS wins in a
row over the weekend. Three wins is not evidence; the bias was measured
across 1,180 matches, where the method predicted BTTS-yes at 54.3%
against a realised 58.1%. A bet that wins half the time at around 2.00
is roughly break-even, not edged — and "does BTTS No win?" was never the
question. The question is whether it wins *more often than the price
implies*, and the measurement says our estimate of that is systematically
too high.

The pause stands.

## Past weeks

- [Matchweek 4](reports/matchweek-4.md) — conclusion book -£14, Codex
  solo +£8.75 on paper
