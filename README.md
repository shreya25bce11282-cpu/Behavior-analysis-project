# Behavior Analysis Project

## Abstract
Mood regulation is closely linked to sleep and cognitive functioning, yet is difficult to measure directly in behavioral datasets. This project examines the relationship between sleep quality, sleep duration, and stress levels, using stress as an operational proxy for mood. Through exploratory analysis and multivariate linear regression, sleep quality emerges as a substantially stronger predictor of stress than sleep duration. Interpreted through cognitive load theory and working memory limitations, the findings suggest that sleep quality affects mood-related outcomes by influencing cognitive efficiency rather than total rest time. The study highlights both the value and limitations of proxy-based behavioral analysis and informs human-centered technology design aimed at reducing cognitive overload and stress.


## Project Structure
- `docs/` — Psychology notes and conceptual background  
- `data/` — Raw and processed datasets used in the analysis  
- `notebooks/` — Jupyter notebooks for data cleaning, EDA, and machine learning models  
- `src/` — Source code reserved for future extensions and applications  

## Dataset
The dataset includes information such as:
- Sleep duration  
- Sleep quality  
- Stress level  
- Physical activity and other lifestyle factors  

The cleaned dataset is stored under `data/processed/`.

## Methods Used
- Descriptive statistics  
- Correlation analysis  
- Data visualization  
- Linear Regression  
- Multivariate Linear Regression  
- Decision Tree Regression  

## Key Findings
- Sleep quality shows a strong negative relationship with stress level.  
- Better sleep quality is associated with lower stress.  
- Multivariate regression indicates sleep quality has a stronger influence on stress than sleep duration.  
- Decision Tree regression achieved high performance, though linear models were preferred for interpretability.
- Sleep duration and sleep quality are strongly correlated; however, sleep quality shows a much stronger negative relationship with stress. This suggests that the effect of sleep duration on stress is largely indirect and mediated through perceived sleep quality.

## Goals
- Build foundational skills in AI/ML and psychology  
- Apply psychological concepts to real-world behavioral data  
- Develop research-oriented projects for higher studies and international applications  
- Establish a base for future work in behavior analysis and applied machine learning  

## Future Scope
This project can be extended by incorporating additional mood indicators,
longitudinal sleep data, or interactive visualizations for deeper behavioral insights.
