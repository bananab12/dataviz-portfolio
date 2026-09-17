---
title: "What grows: the scoring race across the season"
---

**Question.** The final figure "27 goals" hides the interesting part — when those
goals actually arrived. Who led in winter, who closed the gap in May, and who
simply kept an even pace across all 38 matchweeks?

![Running total of goals for the five leading scorers](specs/pl-race.vl.json)

**Decision.** Cumulative lines rather than bars of goals per matchweek: in the
per-round view roughly 80% of the values are zero and the chart turns into a sieve.
The running total makes the plateaus (droughts) and the steps (braces) visible.
Interpolation is linear, with no smoothing — a smoothed curve would draw goals into
weeks where there were none. Five players is the limit before the lines turn into
spaghetti; each one is labelled at its end, so colour is never the only way to tell
them apart.

**What it shows.** Haaland breaks clear after matchweek 10 and never gives the lead
back — not a burst, but a steady rate with no long pauses. Igor Thiago, by
contrast, has two visible plateaus (matchweeks 12–18 and 24–28) and still finishes
second on 22. The most interesting part is at the bottom: Watkins, João Pedro and
Gibbs-White run almost the whole season together and only separate in the closing
rounds. And a counterpoint to the title: nothing "grew" in the league itself — 2.77
goals per match in the first half of the season against 2.73 in the second. What
grows is not league scoring, but individual tallies.
