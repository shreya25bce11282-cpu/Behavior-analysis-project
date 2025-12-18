# Behavior Analysis Project

## Abstract

Mood regulation is closely linked to sleep and cognitive functioning, yet mood is difficult to measure directly in behavioral datasets. This project investigates the relationship between sleep quality, sleep duration, and stress levels, using stress as an operational proxy for mood. Through exploratory data analysis and multivariate linear regression, sleep quality emerges as a substantially stronger predictor of stress than sleep duration. Interpreted through cognitive load theory and working memory limitations, the findings suggest that sleep quality affects mood-related outcomes by influencing cognitive efficiency rather than total rest time. The project highlights both the strengths and limitations of proxy-based behavioral modeling and provides insights relevant to human-centered technology and cognitive science.

---

## Motivation

Understanding human behavior requires bridging psychology with quantitative analysis. Sleep is a fundamental biological process that directly affects attention, memory, emotional regulation, and stress. While mood is a complex and subjective construct, stress provides a measurable behavioral proxy that allows computational analysis. This project was designed as a first step toward combining psychology, machine learning, and behavioral data analysis with an eventual focus on HCI and cognitive science.

---

## Dataset

The dataset contains self reported measures related to sleep and lifestyle, including:

* Sleep duration
* Sleep quality
* Stress level

Stress is treated as a proxy variable for mood, an approach that is explicitly discussed as a methodological limitation in the documentation.

---

## Methods

1. **Data Inspection and Cleaning**

   * Selected relevant variables related to sleep and stress
   * Renamed columns for clarity and consistency
   * Saved a cleaned dataset for reproducibility

2. **Exploratory Data Analysis (EDA)**

   * Visualized relationships between sleep variables and stress
   * Examined correlations among sleep duration, sleep quality, and stress level

3. **Machine Learning Models**

   * Simple linear regression: Sleep Quality → Stress Level
   * Multivariate linear regression: Sleep Quality + Sleep Duration → Stress Level
   * Evaluated models using MSE and R²

---

## Key Findings

* Sleep quality shows a strong negative relationship with stress.
* Sleep duration alone has a weaker relationship with stress.
* In multivariate regression, sleep quality dominates sleep duration as a predictor.

These findings align with cognitive load theory: sleep quality affects how efficiently the brain processes information, whereas sleep duration reflects time asleep without guaranteeing neural recovery.

---

## Psychological Interpretation

The results are interpreted using concepts from cognitive psychology:

* **Working memory limitations** (≈4 chunks)
* **Cognitive load theory** (intrinsic, extraneous, germane load)
* **Attention and emotional regulation**

Poor sleep quality increases cognitive load and reduces executive control, leading to heightened stress even when sleep duration is adequate.

---

## Limitations

* Mood is not measured directly; stress is used as a proxy.
* The dataset relies on self reported measures.
* Linear models capture associations, not causality.

These limitations are acknowledged and discussed in the documentation.

---

## Project Structure

```
Behavior-analysis-project/
│
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   └── sleep_stress_regression.ipynb
├── docs/
│   ├── psychology_intro.md
│   ├── mood_operationalization.md
│   ├── data_inspection.md
│   ├── data_cleaning_notes.md
│   └── final_conclusion.md

└── README.md
```

---

## Skills Demonstrated

* Behavioral data cleaning and analysis
* Machine learning with interpretability
* Psychological theory integration
* Research style documentation

---

## Future Directions

* Extend models to include attention or productivity related variables
* Explore non linear or interaction effects
* Translate findings into HCI design guidelines for stress-reducing interfaces

---

## Long Term Goal

This project is part of a broader portfolio combining psychology, AI/ML, and human-centered design, aimed at preparation for advanced study in Cognitive Science or HCI.
