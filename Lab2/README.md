# The Illusion of Growth & the Composition Effect  
*Deflating History with FRED*

## Objective
This project builds a reproducible Python data pipeline to analyze long-run wage growth in the United States and to correct for misleading statistical signals. Using live data from the Federal Reserve Economic Data (FRED) API, the goal is to move beyond nominal wage growth and investigate whether workers’ **real purchasing power** has meaningfully improved over time—while identifying and correcting for structural measurement biases.

## Methodology
- **Live Data Ingestion (API-Driven):**  
  Leveraged the FRED API (`fredapi`) to pull nominal average hourly earnings (AHETPI) and Consumer Price Index (CPI) data directly from the Federal Reserve, ensuring up-to-date and transparent sourcing.
- **Real Wage Construction:**  
  Deflated nominal wages using CPI to construct a real wage series and evaluate long-term purchasing power rather than headline pay growth.
- **Anomaly Detection (2020 Spike):**  
  Identified an abnormal surge in real wages during 2020 that contradicted labor-market fundamentals.
- **Composition Effect Correction:**  
  Retrieved the Employment Cost Index (ECI), a fixed-composition wage measure, to control for labor-force shifts and isolate true wage dynamics from statistical distortion.
- **Visualization & Comparison:**  
  Indexed and plotted standard average wages against the ECI to directly compare biased versus composition-adjusted wage growth.

## Key Findings — *The Pandemic Paradox*
- Despite steady nominal wage increases over the past five decades, **real wages remain largely flat**, illustrating the persistent “money illusion.”
- The apparent wage boom during the COVID-19 pandemic was **not a genuine increase in labor compensation**.
- The spike was driven by a **composition effect**, as lower-wage workers disproportionately exited the labor force, mechanically raising the average wage.
- The ECI revealed **stable, modest wage growth**, confirming that the 2020 surge in standard wage measures was a statistical artifact rather than an improvement in worker welfare.

**Core Insight:**  
Headline wage statistics can be deeply misleading without proper deflation and composition controls. Correct measurement fundamentally changes the narrative of wage growth in the U.S. economy.
