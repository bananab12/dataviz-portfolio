---
heading: "About the data"
---

Every piece of work on this page is built on one open dataset: player-level match
statistics from the English Premier League, season 2025/26. These are open,
educational data about public sporting events — no work, client or personal data
appears here.

**What is inside.** 11,492 rows, each one player in one match. 380 matches, 38
matchweeks, 20 clubs, 537 players. Each row carries 39 fields: minutes, goals,
assists, shots and shots on target, penalties, cards, fouls, tackles won and
interceptions, plus match attributes — date, matchweek, opponent, venue, attendance
and referee.

**What had to be cleaned.** Three clubs are named differently in the team field and
in the home/away fields: "Brighton" against "Brighton & Hove Albion", "Manchester
Utd" against "Manchester United", "Wolves" against "Wolverhampton Wanderers".
Without reconciling those names, every home-versus-away calculation loses 143 goals
— that is exactly the gap the first sanity check on the totals revealed. The
position field holds several labels separated by commas (for example "FW,AM"), so
grouping uses the first, primary one. Long club names are shortened on the charts
for readability.

**What the data stay silent about.** There are no expected goals (xG), no
possession, no shot locations, so "conversion" in this work is simply goals divided
by shots, not a measure of chance quality. Own goals (40 across the season) are
recorded separately and credited to no player: 1,045 goals were scored in the
matches, 1,005 of which have a named scorer. Penalties are included in the goal
totals but shown separately in the tooltips — 77 scored from 92 attempts.

**How it was built.** The first piece of work is Tableau Public. The rest are
Vega-Lite specifications stored in the `specs` folder of this repository: the data
inside them are pre-aggregated, so the charts render in the reader's browser with no
server involved. Colours come from a single palette shared across all the work and
checked for colour-blind separation; ordered scales (player positions) use one blue
gradient, categories use a fixed set of hues.
