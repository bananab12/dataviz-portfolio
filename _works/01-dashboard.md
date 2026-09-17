---
title: "Club profile: one filter, three views"
wide: true
---

**Question.** The season is over, and the table has twenty team rows — and so what? Every
club answers three different questions at once: who produces the output, how was the journey
through the season, and whether actual scoring output justifies the number of shots taken. My dashboard tries to answer all three points in one report.

![Club profile](specs/pl-dashboard.vl.json "wide")

**Decision.** Three charts on one dataset with one shared filter — the club
selector. On the left, horizontal bars split each player into goals and assists,
because "who produces the output" is a question about both the finish and the pass
before it. On the right, cumulative lines for goals scored and conceded. Below, a
scatter plot with the league's average conversion rate drawn as a dashed line — the
distance of a dot from that line is the verdict on a single player. The shot and goal
scales are identical for every club: give each its own scale, and Wolves would look
like Man. City. 

**What it shows.** Arsenal (as the Champion) scored 67 and conceded just 26 — the
best defence in the league; its conceded line is nearly flat from matchweek 30
onward. Switch to Manchester City, and you see a different build-up: 74 goals,
27 of them from one man, his dot sitting far above the dashed line. Wolves are the
mirror image: 26 goals and a 7.0% conversion against a league average of 10.6% —
the same volume of shooting, far less end-to-end productive.
