# 📈 The Cost of Living Crisis: A Data-Driven Analysis

## The Problem
Headline inflation, as measured by the official Consumer Price Index (CPI), is often treated as a universal indicator of cost-of-living pressures. However, this “average” measure obscures how inflation is actually experienced by specific populations. For students, spending is heavily concentrated in categories like tuition, rent, and food away from home—categories that historically inflate faster than the national average. As a result, relying solely on official CPI systematically understates the real financial pressure faced by students.

---

## Methodology
This project combines manual data construction with official economic data from the Federal Reserve Economic Data (FRED) API. I first constructed a representative “student basket” to illustrate category-specific inflation between 2016 and 2024. I then fetched CPI sub-indices for tuition, rent, food away from home, and subscriptions, alongside the national CPI benchmark.

All series were re-indexed to a common base year (2016 = 100) to correct for differing CPI base years—a necessary step given that CPI indices are Laspeyres-style price indices with heterogeneous reference points. I then constructed a custom **Student-Specific Price Index (Student SPI)** by reweighting components to reflect realistic student spending patterns, placing greater weight on tuition and housing. Visualization and analysis were performed in Python using pandas and matplotlib.

---

## Key Findings
My analysis reveals a substantial divergence between student-experienced inflation and national inflation. While the official CPI suggests moderate long-run price growth, the Student SPI rises significantly faster after 2016, driven primarily by tuition and rent inflation.

Additionally, a comparison between national CPI and regional CPI (Boston–Cambridge–Newton) shows that students in high-cost metropolitan areas experience even greater inflationary pressure, compounding affordability challenges.

---

## Why It Matters
This analysis demonstrates that inflation is not a uniform phenomenon. Aggregate indices can mask meaningful variation across demographic groups and regions. Understanding student-specific inflation is essential for informed policy design, financial aid decisions, and cost-of-living adjustments.

---

### 🔧 Tools & Skills Demonstrated
- Python (pandas, matplotlib)
- API data ingestion (FRED / fredapi)
- Index construction & normalization (Laspeyres framework)
- Applied macroeconomic analysis
- Data visualization & economic storytelling
