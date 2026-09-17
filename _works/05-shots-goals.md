---
title: "Are they related: what a goal costs in shots"
---

**Question.** "Shoot more and you will score more" sounds self-evident. How strong
is that relationship really, and who falls outside it in either direction?

![Shots and goals for players with 15+ shots in the season](specs/pl-shots-goals.vl.json)

**Decision.** A scatter plot is the only form that shows the relationship between
two quantities and the individual cases at the same time. The dashed line is not a
regression line but the league's average conversion (10.6% of shots) — a reference
anyone can interpret: above it, a player scores more than his attempts "entitle"
him to. The colour splits the dots on exactly that boundary, and the boundary is
named in the legend rather than left to be guessed. The minimum-shots slider strips
out the tail of accidental values: a player with three shots and one goal has a
"33% conversion" that means nothing. Only three dots are labelled — the two poles
and the sharpest counter-example; labelling all of them would make the chart
unreadable.

**What it shows.** The link is strong but not ironclad: the correlation between
shots and goals is 0.82, while between shots **on target** and goals it is 0.90. It
is accuracy, not activity, that counts — the difference between "covered a lot of
ground" and "produced a result". Haaland (126 shots, 27 goals) and Thiago (84 and
22) sit far above the dashed line, each roughly 13 goals above the expected rate.
Viktor Gyökeres scored 14 from 55 shots — 25%, the best conversion among the leading
scorers. At the bottom sits David Brooks: 48 shots, one goal. For a finance person
this is a familiar picture: activity is easy to measure and easy to mistake for
results, which is why every report that shows "attempts" must show "hits" next to
it.
