# Czech Lifestyle Decision Dashboard

PostgreSQL + Power BI Project

Persona-based city ranking model built with PostgreSQL scoring logic and Power BI analytics.

---

Choosing where to live depends on priorities. A student, an IT professional, and a family evaluate a city differently.

This project builds a weighted scoring model that ranks Czech cities based on persona-specific preferences. Instead of presenting raw indicators, it calculates a structured score and highlights the main factors influencing each ranking.

---

## What This Project Does

- Compares cities using multiple lifestyle indicators  
- Applies different weights depending on the selected persona  
- Produces a final weighted score per city  
- Identifies the top 3 factors driving each score  

---

## How It Works

The data model follows a star-schema structure.

Core tables:
- `fact_persona_scores`
- `fact_top_reasons`

Supporting dimensions:
- City  
- Persona  
- Month  
- Metric  
- Source  

All transformations and scoring logic are implemented in PostgreSQL.  
Metrics are normalized before weights are applied to ensure comparability.

Final score formula:

Weighted Score = Σ (Normalized Metric × Persona Weight)

---

## Dashboard

The Power BI report allows interactive exploration by:

- Persona  
- Month  
- City  

Users can compare rankings, analyze trends, and understand the main drivers behind each result.

---

## Tools

PostgreSQL  
SQL  
Power BI  
GitHub  

---

Kirannjot Kaur  
Computer Science Student – Data & Analytics
