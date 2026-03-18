# Healthcare Patient Risk Analytics Dashboard — Power BI

## Business question
Which patient profiles, departments, and hospital regions carry 
the highest risk burden — and what does that mean for capacity 
planning and resource allocation?

## Dataset
Healthcare Analytics Dataset — 318,438 patient records across
multiple hospitals, departments, and regions (Kaggle public domain).
Columns: admission type, severity of illness, department, 
hospital region, length of stay, admission deposit.

## Methodology
- Built a 4-tier Risk Classification model combining two variables:
  Severity of Illness + Type of Admission
- Critical Risk = Extreme severity + Emergency admission
- High Risk = Extreme severity (non-emergency)
- Medium Risk = Moderate severity
- Low Risk = Minor severity
- Calculated Critical Risk % per hospital region for 
  geographic risk comparison
- Findings structured as 3 prioritised audit observations

## Key findings
1. CRITICAL RISK — 6.23% of all cases (19,844 patients) qualify 
   as Critical Risk. Gynecology carries the highest case volume 
   with disproportionate risk concentration.
2. REGIONAL DISPARITY — Region Y carries the highest critical 
   risk rate at ~63% vs Region X at ~30%, indicating uneven 
   resource allocation across the hospital network.
3. CAPACITY PRESSURE — 62% of patients stay 21+ days. 
   Long-stay cohort represents the highest bed-blocking 
   and cost risk for the system.

## Tools used
Power BI Desktop · DAX (calculated columns and measures) · 
Conditional formatting · Interactive slicers

## Files
- `train_data.csv` — source dataset
- `HSE Dashboard.pbix` — Power BI file
- `dashboard-screenshot.png` — dashboard preview

## Dashboard preview
![Dashboard](dashboard-screenshot.png)
