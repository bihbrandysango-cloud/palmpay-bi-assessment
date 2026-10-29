# Palmpay sales analysis

![Palmpay sales analysis](06%20Logo%20and%20Cover/Cover%20image.png)

Power BI report and presentation answering the Palmpay Business Intelligence Analyst assessment: five years of sales (2007 to 2011) in the United States and Germany.

Built by Bih Brandy Sango.

## About this version

I first answered this assessment in October 2025. This repository holds the rebuild I made in October 2026, after studying Power BI and Fabric. It is a 12-page report in the Power BI Project (.pbip) format, so every page, measure and relationship is readable as text. The 2025 files are not included.

## What the data says

| Question | Answer |
|---|---|
| Overall | $285M revenue, $149M gross profit, 52.3% margin, about 169,000 items sold |
| A1, A2: the two countries | Germany grew every year, from $31.0M to $35.1M. The US fell from $28.0M in 2008 to $20.8M in 2009 and has stayed near $21.5M since |
| A3: the 2008 crisis | Sales were 11.6% below the year before in September 2008 and 24.2% below in January 2009 (excluding Silicon Valley Bikes). The US fell as far as 45.9%; Germany's worst month in 2008 and 2009 was -9.8% |
| B1: the flop | Fixed Gear Bike Plus, with 21, 17, 10, 10 and 14 units a year (72 in total) |
| B2: top category | Touring bikes in every year, 37 to 40% of revenue |
| B3: off-road bikes by city | 37.5% of 2011 bicycle units. München (48.7%), Denver (48.0%) and Irvine (41.1%) are the highest |
| B4: seasonality | 54% of revenue arrives in April to June. The First Aid Kit is the one product without a season |
| B5: recommendations | Win back US customers, rethink US discounts, keep investing in the three main bike lines, review the Fixed Gear Bike Plus, plan around the season |

All figures are in US dollars. The source sheet records sales in more than one currency, and the dollar columns are the only fair way to compare the two countries.

## What is in the project

- `01 Strategic Brief.pdf` explains the audience, the message and the slide-by-slide storyline.
- `02 Presentation.pptx` is the 11-slide deck, with the speech in the slide notes.
- `03 Speech.md` is the same speech as a text file (about 9 minutes spoken), with answers to likely questions.
- `04 Power BI Report/` holds the report and semantic model as a Power BI Project.
- `05 Report Screenshots/` has an image of each of the 12 report pages.
- `06 Logo and Cover/` has the Palmpay logo used in the report and the deck, and the cover image.

## The report

The twelve pages follow the assessment: introduction, executive overview, US vs Germany, monthly sales against the previous year, the crisis side by side, top category and slowest product, top cities and product mix, seasonality, two drill-through pages (city and product), key findings, and recommendations.

Features I added while studying:

- KPI cards with 12-month sparklines
- Chart titles that change with the selected year, and reference lines driven by measures
- A metric switcher (revenue, units sold, gross margin) built on a field parameter
- City and product drill-through pages
- Data bars in the tables
- Anomaly detection on the year-on-year chart
- Small multiples for the crisis comparison
- A play axis that steps through the years on the overview, top category and seasonality pages

## Opening the report

You need Power BI Desktop. Open `04 Power BI Report/Palmpay Sales.pbip`.

The sales data is not included, because the Excel workbook belongs to the assessment. The model still points to the original file path, so choose Transform data and set the Excel source to your own copy before refreshing. The Play Axis visual comes from AppSource and installs the first time Power BI asks for it.
