---
heading: "About the data"
---
Every piece of work on this page is built on one open dataset: player-level match
statistics from the English Premier League, season 2025/26. These are open,
educational data about public sporting events — no work, client, or personal data
appears here.

**What is inside?** 11,492 rows, each one player in one match. 380 matches, 38
matchweeks, 20 clubs, 537 players. Each row carries 39 fields: minutes, goals,
assists, shots and shots on target, penalties, cards, fouls, tackles won and
interceptions, plus match attributes — date, matchweek, opponent, venue, attendance
and referee.

**How was it built?** The first piece of work is Tableau Public. The rest are
Vega-Lite specifications stored in the `specs` folder of this repository: the data
inside them are pre-aggregated, so the charts render in the reader's browser with no
server involved. 
