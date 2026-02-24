# fvsd-education-analytics-powerbi
# Education Performance & Resource Planning Dashboard
## Sources:
![alt text](image.png)

https://zoomcharts.com/en/microsoft-power-bi-custom-visuals/challenges/fp20-analytics-january-2024
## Project Overview
This Power BI dashboard was developed to support academic monitoring, intervention staffing allocation, and testing cost forecasting within an education environment.

The model connects student assessment performance directly to workforce planning and financial impact, enabling data-driven operational decisions.

---

## Business Objectives
The dashboard addresses three primary decision areas:

1. Academic performance monitoring  
2. Tier 2 / Tier 3 intervention staffing allocation  
3. Testing cost forecasting and budget planning  

---

## Key Executive Insights

### Academic Performance
- Performance follows cyclical semester patterns (Spring peak, Fall baseline).
- No structural academic decline observed.
- Early grades (Grade 1–3) show highest intervention demand.

### Cost Structure
- Testing cost increases are volume-driven, not price-driven.
- Grades 2–3 generate the highest total assessment cost.
- Cost concentration aligns with enrollment distribution.

### Enrollment Dynamics
- Enrollment declines significantly from Grade 10 onward.
- Population shifts directly impact staffing demand and cost projections.

---

## Analytical Framework

### Academic Monitoring Layer
KPIs analyzed:
- Average Standard Score by Semester
- % Assessment Level Distribution
- % Below Average vs Average & Above
- Tier 2 / Tier 3 student counts

### Cost Allocation & Efficiency
- Total Cost by Assessment Type
- Cost by Grade & School
- Cost per Student
- Cost Trend Over Time

Scatter analysis confirms cost scales proportionally with enrollment volume.

---

## Forecasting & Workforce Planning Logic

A critical modeling distinction was identified:

Distinct student counts across semesters  ≠ Average distinct student count per semester

        Correct Forecast Formula:
        (Sem1 + Sem2 + Sem3) / 3

        Incorrect logic (DistinctAcrossAll / 3) would underestimate staffing demand.

### Forecasting Models Evaluated
1. 3-Semester Rolling Average (stable smoothing approach)
2. Delta % Change Model (trend-responsive)

Example Impact:
A 20-student forecast gap equals approximately 2 teachers (10:1 Tier 2 ratio).

---

## Technical Skills Demonstrated
- Star schema data modeling
- Custom academic calendar
- Advanced DAX (DISTINCTCOUNT, AVERAGEX, Delta logic)
- Time intelligence for non-standard fiscal calendars
- Forecast scenario comparison modeling
- Business-oriented analytical storytelling

---

## Author
Tran Nguyen  