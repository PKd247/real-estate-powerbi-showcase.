# Real Estate Power BI Showcase

*Consistent, decision-ready Power BI reporting for real estate, generated from code instead of built by hand.*

By [Prem Kumar Loganathan](https://www.linkedin.com/in/premkumarloganathan/), founder of [d247 consulting](https://www.d247consulting.in).

> **Note:** This repository is a showcase. All figures and screens come from a **demo dataset** designed to behave like a real business. No client data is shown. The full project is kept in a private repository.

---

## The idea

Every report built by hand is another chance for a mistake: a wrong currency label, a page that scrolls, a missing logo. This suite avoids that by generating every report from code, and checking each one against a rulebook before it is saved.

## The suite at a glance

| Layer | What it contains |
|---|---|
| **Data** | 68 CSV tables covering off-plan sales, handovers, leasing and resale, all linked by unit |
| **Model** | Star schema in TMDL: 22 facts, 51 dimensions, 151 relationships |
| **Measures** | 907 DAX measures following one set of conventions |
| **Reports** | 39 Power BI reports |
| **Documentation** | Client guide (Word and PDF), developer guide, screenshots and walkthrough videos |

|<img width="960" height="540" alt="pipeline" src="https://github.com/user-attachments/assets/1497774e-4061-4217-8b67-48bb2c7a0812" />


## How it works

1. **Data design.** The dataset is built to behave like a real business. Every status is a dated event, one unit can move through sale, handover, leasing and resale, and the profit and loss is derived from deals, installments, payroll and marketing spend.
2. **Model.** Rules are applied the same way every time: column types from naming patterns, relationships by display name, a local date table with public holidays and Ramadan, and one folder parameter that points all reports at the data.
3. **Measures.** Operational measures stop at today, P&L stops at the last closed month, and comparisons use the same days of the prior year. Formats include ▲ and ▼ trend arrows, and some measures return SVG sparklines or story subtitles.
4. **Reports.** Each report is defined by one specification file. Running the build produces a complete Power BI project with every page, visual, bookmark and theme.
5. **Documentation.** Manifests record every page and visual, so the guides write themselves.

!<img width="960" height="540" alt="report-gallery" src="https://github.com/user-attachments/assets/9e1f992c-cfc7-4ccc-916d-cb440332c369" />


## Quality gate

A rulebook runs on every build. If a rule fails, the build names it and nothing is written. Examples of what it enforces:

- Local time on every page
- Help text on every visual
- USD only, never a bare `$`
- A single font (Segoe UI)
- Pages that never scroll
- A click filters, it never only highlights
- Every measure used by a report exists in the model

## Example reports

!<img width="960" height="540" alt="report-spec" src="https://github.com/user-attachments/assets/566d2b99-75f4-4cf1-8f70-8a2e54da9ab0" />


Reports in the suite include Metric Explorer, Agent Profile, Income Statement, Lead Quality, Project Schedule, Landlord Statement, Price Changes, KYC Overview, Lease Renewals Due, and Occupancy and Vacancy.

## Model lineage

An Obsidian vault maps how everything connects, from the semantic model to its tables and reports. Before a table is changed, you can see which reports it feeds.

## Who it's for

- Property developers
- Brokerages and agencies
- Property managers and landlords

## let's connect

If you'd like clear, consistent reporting for your real estate business, let's talk.

- 💼 LinkedIn: [in/premkumarloganathan](https://www.linkedin.com/in/premkumarloganathan/)
- 🌐 Website: [www.d247consulting.in](https://www.d247consulting.in)
- 📍 Chennai, India
