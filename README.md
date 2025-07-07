# Chicago Food Inspections & Business Licenses Audit

This project, developed as part of the University of Chicago Data Engineering program, investigates the relationship between food inspection outcomes and business license statuses in Chicago. It uses Python, SQL, and relational database design to analyze whether inspection failures lead to regulatory actions like license suspensions or revocations.

## Project Objectives

- Determine if inspection outcomes (failures, violations) impact the status of business licenses.
- Assess whether inspections can be reliably linked to business licenses.
- Identify businesses operating without valid licenses.
- Provide actionable, data-driven insights to improve public safety and regulatory compliance.

## Dataset

Data was sourced from the City of Chicago Open Data Portal (2020–2025):
- Food Inspections Dataset
- Business Licenses Dataset

## Key Technologies

- Python (ETL, data cleaning, visualization)
- MySQL (relational database, query analysis)
- SQL (data integration, querying)
- Pandas, Matplotlib, Seaborn (visualization)

## Project Structure

- `GregBandy_FinalProject.ipynb` - Full Jupyter Notebook with Python ETL pipeline, SQL queries, and visualizations.
- `DataEngineeringReport_GregBandy.pdf` - Formal project report with methodology, relational schema, SQL findings, and visualizations.
- `README.md` - Project documentation.

## Methodology

- Built a normalized relational database (3NF) linking inspections, licenses, businesses, violations, and locations.
- Developed Python-based ETL to clean and structure the datasets.
- Created an Enhanced Entity Relationship (EER) diagram to visualize table linkages.
- Used SQL queries and Python visualizations to uncover trends, mismatches, and regulatory gaps.

## Key Findings

- **Linkage Gaps:** Many inspections could not be reliably matched to licenses, highlighting system inconsistencies.
- **Compliance Issues:** Thousands of businesses were found to be operating without active licenses.
- **Enforcement Gaps:** Businesses with repeated violations often retained active licenses.
- **Timing Mismatches:** License expiration dates and inspection schedules are poorly aligned.
- **Geographic Trends:** Identified ZIP codes with high concentrations of active businesses.

## Visualizations

- Top violators by total and average violations.
- Trends in monthly inspections and violations.
- Heatmaps of active businesses by ZIP code.
- License expirations by month.
- Inspection results by license status (pass/fail).

## Recommendations

- Automate enforcement triggers for failed inspections.
- Synchronize inspection and licensing systems across city departments.
- Develop an `enforcement_actions` dataset to track regulatory responses.
- Digitize revocation workflows to automate license suspensions.
- Standardize key fields to improve data linkage.

## Lessons Learned

- Data normalization and unique identifiers are critical for database integrity.
- SQL and relational design are powerful but need to be paired with visual storytelling for policy impact.
- Python-based dashboards and visualizations are viable alternatives to commercial BI tools.
- Regulatory datasets often lack real-time integration, creating blind spots in enforcement.

---

## How to Use

### Prerequisites
- Python 3.x
- MySQL
- Required libraries:
```bash
pip install pandas numpy matplotlib seaborn sqlalchemy
