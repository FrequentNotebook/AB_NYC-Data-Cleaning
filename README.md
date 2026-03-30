# AB_NYC_2019 — Airbnb NYC 2019 Data Analysis

End-to-end data analysis of 48,895 Airbnb listings in New York City, covering data cleaning, exploratory data analysis, and honest interpretation of findings.

---

## Project Structure

| Notebook | Description |
|---|---|
| `AB_NYC_2019_Data_Cleaning.ipynb` | Data cleaning pipeline — 48,895 → 48,768 rows, 127 rows dropped across three cleaning operations |
| `AB_NYC_2019_EDA.ipynb` | Univariate and multivariate analysis covering price, availability, reviews, borough distribution, and host behaviour patterns |

---

## Key Findings

**Pricing**
- The typical NYC listing costs **$105 (median)** — the mean of $153 is distorted by luxury outliers up to $10,000
- Price is strongly tied to room type: entire homes ($160) cost more than double private rooms ($70) and over triple shared rooms ($45)
- Manhattan is the most expensive borough ($150 median) and the most listed (21,592 listings)

**Listings Distribution**
- Manhattan and Brooklyn together account for **85.4% of all listings** — the market is geographically concentrated
- Staten Island is physically isolated and severely underrepresented (373 listings) despite having the highest median review count (20)

**Availability**
- **35.9% of listings have zero availability** — over 1 in 3 listings are either fully booked, paused, or blocked
- Active listings cluster at two extremes: very low availability (1–10 days) or fully open (365 days)

**Reviews**
- **20.4% of listings have never been reviewed** — 1 in 5 listings has no booking history
- Staten Island's low competition explains its high median reviews, while Manhattan's high competition suppresses its median (8)
- Price and reviews have a weak negative correlation (−0.04) — price alone does not predict booking activity

**Host Behaviour**
- Only **0.92% of hosts own more than 5 listings**, yet they control **9.66% of all listings**
- Multi-hosts charge more for entire homes ($175 vs $151) but less for shared rooms ($38 vs $65) — professional hosts price to maximise occupancy, personal hosts price their space as personal

---

## Tools

Python, pandas, matplotlib, seaborn, Jupyter

---

## Dataset

[AB_NYC_2019 — Kaggle](https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data)
