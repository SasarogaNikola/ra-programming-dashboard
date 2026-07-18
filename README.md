
# RA Programming Dashboard — Power BI

## Overview

I built this dashboard to track and evaluate Resident Assistant (RA) programming across the academic year — every event we ran, who worked it, how much it cost, and how it tied back to each RA's performance. The goal was to turn a semester's worth of scattered event logs into something a supervisor could actually use to make decisions.

## How the scoring worked

Each RA earned points across four categories every month: door decorations, bulletin boards, event programming, and event pictures (documentation that the event actually happened as planned). Points from each category rolled up into a monthly total, which is what drives the Top RAs by KPI ranking on the dashboard.

Starting in January, I introduced a monthly **RA League** — a lightweight competition that ranked RAs by category (door decorations, event flyers, event attendance, and bulletin boards) and publicly recognized the top performer in each. It was a small change, but it mattered: you can see the effect directly on the Average Attendance by Month chart. November shows a clear dip, which lines up with a stretch of lower recognition and lower motivation before the league existed. Once the league started, attendance trended back up through the spring.

## What the data showed

A few patterns stood out once the numbers were in front of me instead of scattered across spreadsheets:

- **Social events tagged with the "Joy" Franciscan value consistently drew the largest crowds.** That combination outperformed every other pairing of learning outcome and value, which is why I'm planning to lean into more social/joy-themed programming next year rather than spreading the budget evenly across categories.
- **Cost and popularity were linked.** The RAs and events that landed at the top of the rankings also tended to have higher cost per event. Popularity wasn't free — the events people actually showed up for were generally the ones we invested more in, not the low-cost ones.
- **KPI scores turned out to be a genuinely useful signal, not just a scoreboard.** I used them to help decide who to consider for rehire the following year, and on the flip side, RAs with lower scores got more of my direct attention and support rather than being written off — the point was to catch it early and help, not just rank people.

## A note on the data

Attendance, points, and event details are all real records from the semester. **Cost figures are approximate** — I estimated them where receipts weren't itemized per event, so treat the cost/attendee number as directional rather than exact accounting.

## Tools

Data was cleaned and modeled in Excel, then built out in Power BI with a small star schema (Events, RA Roster, KPI) connected through a shared RA dimension table, with DAX measures for the derived metrics like Cost per Attendee.
