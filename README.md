Czech Lifestyle Decision Dashboard
PostgreSQL + Power BI Analytical Project

Project Overview
This project explores how different types of people would rank Czech cities based on what matters most to them.
A student, an IT professional, and a family don’t evaluate a city the same way.
Instead of looking at raw numbers, this model calculates a weighted score for each city based on persona-specific priorities.
The result is a structured, explainable ranking system that shows not only which city ranks highest — but why.

Objective
To build a transparent decision-support model that:
Compares Czech cities across multiple lifestyle indicators
Applies different weights depending on the selected persona
Produces a final score per city
Highlights the top contributing factors behind each ranking

Data & Modeling Approach
The project is built using a structured star-schema design.

Core Tables
fact_persona_scores – final weighted score per city, persona, and month
fact_top_reasons – top 3 metrics contributing to each score

Dimensions
City
Persona
Month
Metric
Source

All scoring logic is handled in PostgreSQL using normalization and weighted aggregation.

Scoring Method
Each persona is assigned custom weights.

Example:
Students prioritize affordability and education.
IT professionals prioritize salary and lifestyle.
Families prioritize safety, healthcare, and environment.
Each metric is normalized to ensure comparability.

The final score is calculated as:
Weighted Score = Σ (Normalized Metric × Persona Weight)

This ensures consistent, explainable, and fair ranking.

Dashboard Capabilities

The Power BI dashboard allows:
Interactive persona selection
Monthly trend comparison
City-level ranking
Breakdown of top contributing metrics
Identification of the best city per persona
The focus is clarity and decision support, not visual overload.

Key Observations (Sample Data)
Prague ranks highest for IT professionals due to strong salary and lifestyle indicators.
Ostrava performs better for students because of lower living costs.
Family rankings are driven mainly by safety, healthcare, and pollution levels.

Tools Used
PostgreSQL (data modeling & scoring logic)
SQL (normalization, ranking, aggregation)
Power BI (data modeling, DAX, visualization)
GitHub (project documentation & version control)
