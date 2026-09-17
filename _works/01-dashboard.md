---
title: "Club profile: one filter, three views"
wide: true
---

**Question.** The season is over and the table has twenty rows — now what? Every
club answers three different questions at once: who produces the output, how it
travelled through the season, and whether it really scores as much as its shot
volume suggests. This dashboard answers all three without switching between three
separate reports.

![Club profile](specs/pl-dashboard.vl.json "wide")

**Decision.** Three charts on one dataset with one shared filter — the club
selector. On the left, horizontal bars split each player into goals and assists,
because "who produces the output" is a question about both the finish and the pass
before it. On the right, cumulative lines for goals scored and conceded: not bars
per matchweek, where the noise of a single round drowns the trend, but a running
total that exposes the moment a club started leaking or pulled away. Below, a
scatter plot with the league's average conversion drawn as a dashed line — the
distance of a dot from that line is the verdict on a player. The shot and goal
scales are identical for every club: give each its own scale and Wolves would look
like Manchester City. Pie charts and wall-of-numbers tables were rejected
deliberately — the first make players impossible to compare, the second force you
to read figures instead of seeing the picture.

**What it shows.** Arsenal (the default view) scored 67 and conceded just 26 — the
best defence in the league; its conceded line is nearly flat from matchweek 30
onward. Switch to Manchester City and you see a different construction: 74 goals,
27 of them from one man, his dot sitting far above the dashed line. Wolves are the
mirror image: 26 goals and a 7.0% conversion against a league average of 10.6% —
the same volume of shooting, far less end product. In business terms, that is the
difference between a funnel with too few leads and a funnel with plenty of leads
and a broken conversion rate.
