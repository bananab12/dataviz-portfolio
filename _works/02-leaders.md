---
title: "Who is bigger: who creates the output in the league"
---

**Question.** Who counts as the player of the season — the one who scores or the
one who sets up? The answer depends entirely on the metric, so the right form is
not a single ranking but a ranking with a switch.

![Top 15 of the season by the selected metric](specs/pl-leaders.vl.json)

**Decision.** Horizontal bars with the value labelled at the end and the club next
to the name: the reader gets the order, the numbers and the context without
hovering. The metric switch changes both the value and the membership of the list,
which is more honest than three separate static charts — it shows how different
"the top" can be. Vertical columns were out: player names are long, and on a
vertical axis they would have to be truncated or tilted 45°. Sorting by minutes
played was dropped too — that is a different question and deserves its own chart.

**What it shows.** By goals + assists, Erling Haaland leads with 35 (27 + 8), and
the gap is wide enough that switching metrics barely rescues the chasing pack. But
switch to assists and the top is Bruno Fernandes with 21 assists and nine goals — a
player the scoring charts never notice. Third overall, Igor Thiago scored 22 goals,
eight of them penalties: the tooltip keeps that figure separate, because a penalty
and an open-play goal are worth the same to the club but not to the player.
