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
| Conclusion (debated) | **Yes — actual stakes** | £204.00 | **+£4.00** over 6 bets | £10 on 1 bet |
| Codex solo | **Yes — actual stakes** | £209.59 | **+£9.59** over 3 bets | £40 on 4 bets |
| Claude solo | Tracked only, never staked | £214.25 if funded | +£14.25 on paper | — |
| Cross-book accumulators | **Yes — actual stakes** | n/a, own pot | **-£10.00** (dead — BTTS No leg lost) | — |

**Correction, 20 September 2026:** this table previously described the
Codex book as "tracked only, not staked". That was wrong — it has had
real money through it since Matchweek 5. Its tracked-only figure was
also stale. Totals are now computed from the ledgers by
`scripts/totals.py` rather than maintained by hand, which is how the
drift happened.

Claude solo leads, and it is the one book with nothing staked on it.
Tracked figures use the price at selection time; the real-money figures
use the price actually obtained. Two gameweeks in, with most of
Matchweek 5 still unsettled — nowhere near enough to call any of this
skill rather than noise, in either direction.

## Matchweek 5 — placed

### Conclusion book (Claude and Codex agreed) — placed, real money

| Fixture | Kick-off | Pick | Price obtained | Result |
|---|---|---|---|---|
| [Tottenham v Aston Villa](reports/matches/2026-09-19-TOT-AVL.md) | Sat 19 Sep, 12:30 | Villa win | 3.80 | **Won** (+£28) |
| [Tottenham v Aston Villa](reports/matches/2026-09-19-TOT-AVL.md) | Sat 19 Sep, 12:30 | BTTS: No | 2.25 | **Lost** (-£10) |
| [Man City v Sunderland](reports/matches/2026-09-20-MCI-SUN.md) | Sun 20 Sep, 14:00 | BTTS: No | 1.70 | pending |

Tottenham 2-3 Aston Villa full time — net **+£18** on this fixture.

Also placed: a **"Bet Builder+" accumulator** (£10, combined price
1724.91/1) covering all ten markets below, conclusion and Codex-solo
mixed together. This initially broke the single-book accumulator rule
set after Matchweek 4 — the rule was amended the same day to allow
cross-book accumulators, since every leg had already independently
cleared its own book's threshold before the acca combined them.
Tracked in its own running total, not charged against either book's
bank.

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
| 1 | [Man City v Sunderland](reports/matches/2026-09-20-MCI-SUN.md) | Sun 20 Sep, 14:00 | Man City win | 1.30 | pending |
| 2 | [Nottingham Forest v Coventry](reports/matches/2026-09-19-NFO-COV.md) | Sat 19 Sep, 17:30 | BTTS: No | 1.91 | **Won** (+£9.09) |
| 3 | [Bournemouth v Liverpool](reports/matches/2026-09-20-BOU-LIV.md) | Sun 20 Sep, 14:00 | Liverpool win | 2.10 | pending |
| 4 | [Bournemouth v Liverpool](reports/matches/2026-09-20-BOU-LIV.md) | Sun 20 Sep, 14:00 | BTTS: No | 2.70 | pending |
| 5 | [Everton v Ipswich](reports/matches/2026-09-19-EVE-IPS.md) | Sat 19 Sep, 15:00 | BTTS: No | 2.05 | **Won** (+£10.50) |
| 6 | ~~Fulham v Man Utd, BTTS: No~~ | Sun 20 Sep, 16:30 | *dropped before placing* | — | — |
| 7 | [Leeds v Crystal Palace](reports/matches/2026-09-20-LEE-CRY.md) | Sun 20 Sep, 14:00 | BTTS: No | 2.05 | pending |
| 8 | [Everton v Ipswich](reports/matches/2026-09-19-EVE-IPS.md) | Sat 19 Sep, 15:00 | Ipswich win | 4.20 | **Lost** (-£10) |
| 9 | ~~Fulham v Man Utd, Fulham win~~ | Sun 20 Sep, 16:30 | *dropped before placing* | — | — |

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

## Past weeks

- [Matchweek 4](reports/matchweek-4.md) — conclusion book -£14, Codex
  solo +£8.75 on paper
