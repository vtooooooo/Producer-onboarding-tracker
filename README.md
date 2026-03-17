# Producer Onboarding Tracker

An end-to-end Excel-based operations tracker built to simulate the 
producer onboarding workflow at an insurance agency. Designed as a 
portfolio project targeting the Producer Services / Operations Analyst 
function at insurance firms like Chubb.

---

## Project Overview

This tracker manages the full lifecycle of insurance producer 
onboarding — from initial application through license verification, 
background checks, and final activation. It is built entirely in 
Microsoft Excel using dynamic formulas, conditional formatting, and 
structured data across five interconnected sheets.

---

## Workbook Structure

| Sheet | Description |
|---|---|
| Agent Master Data | Core dataset of 30 synthetic producers with status, tier, license expiry, and BG check fields |
| KPI Dashboard | Live KPI cards and tier breakdown table driven by Excel formulas |
| License Expiry Alerts | Active agents sorted by expiry date with auto-flagged alert levels |
| BG Check Tracker | All agents sorted by BG check priority with action recommendations |
| Legend & Instructions | Color key, status definitions, and field descriptions |

---

## Key Features

- **Agent Status Pipeline** — Tracks each producer across 6 stages:
  Applied → Under Review → Pending Docs → Active → Rejected → Terminated
- **License Expiry Alerting** — Automatic color-coded flags using
  DATEDIF(TODAY(), ...) with Expired / Critical / Warning / OK tiers
- **Background Check Tracker** — Priority-sorted view with escalation
  actions for Failed and Pending checks
- **KPI Dashboard** — 7 status KPIs + 4 performance metrics including
  avg processing days, rejection rate, and BG check pass rate, all
  driven by COUNTIF / COUNTIFS / AVERAGEIF formulas
- **Tier Breakdown** — Cross-tab of agent counts by Tier × Status
  using COUNTIFS across multiple criteria

---

## Excel Functions Used

`COUNTIF` · `COUNTIFS` · `AVERAGEIF` · `DATEDIF` · `TODAY` · 
`IF` · `IFERROR` · Conditional Formatting Rules · Data Validation · 
Cross-sheet formula references

---

## Dataset

30 synthetic producer records generated for portfolio purposes.
No real agent or insurance data is used.

Fields include: Agent ID, Agent Name, Agency, State, Tier,
Application Date, Status, License Expiry, BG Check Status,
Processing Days, Rejection Reason, Notes.

---

## Business Context

This project is modeled after real responsibilities in a 
Producer Services / Onboarding Analyst role, including:

- Onboarding new producers and maintaining records in internal systems
- Monitoring license verification and background check status
- Tracking enrollment pipeline across tiers
- Supporting audit reporting and trend analysis

---

## Tools Used

- Microsoft Excel (Office 365)
- openpyxl (Python) — used to generate synthetic dataset and 
  workbook structure

---

## File

| File | Description |
|---|---|
| `Producer_Onboarding_Tracker.xlsx` | Main workbook with all 5 sheets |

---

## Author

**Darshan**  
MS Data Science — University of New Haven (May 2026)  
[Portfolio](https://vtooooooo.github.io/portfolio) · [LinkedIn](https://www.linkedin.com/in/vitturamadasudarshan)
