# Behavior Analysis Project

## Overview

This project explores the relationship between **sleep, cognition, and mood-related outcomes** using a combination of **cognitive psychology theory** and **interpretable machine learning models**. The work is positioned at the intersection of **Psychology × Data Science × Human-Centered AI**, with a long term focus on HCI and Cognitive Science research.

Rather than treating machine learning as a black box, this project is **theory-driven**: concepts from attention, working memory, and cognitive load guide the choice of variables, analysis, and interpretation of results.

---

## Research Motivation

From a cognitive psychology perspective, sleep plays a critical role in:

* Neural recovery and synaptic resetting
* Efficient functioning of attention and working memory
* Emotional regulation

Impairments in these systems often manifest subjectively as **stress, irritability, and reduced cognitive control**, which are commonly associated with mood disturbances.

This project investigates whether **sleep quality** and **sleep duration** differ in how strongly they predict stress levels, and why.

---

## Dataset

* Source: Publicly available dataset from Kaggle (Sleep Health and Lifestyle Dataset)
* Nature: Self-reported measures

### Key Variables Used

* **Sleep Duration** (hours)
* **Sleep Quality** (ordinal scale)
* **Stress Level** (ordinal scale)

> **Note on Mood Operationalization:**
> Stress is used as a *proxy measure* for mood related disturbance. This choice is theoretically justified and explicitly discussed as a limitation in `docs/mood_operationalization.md`.

---

## Methodology

The analysis follows a structured, reproducible pipeline:

1. **Data Inspection**
   Understanding variable distributions and potential limitations of self reported data.

2. **Data Cleaning**
   Selecting relevant variables and producing a cleaned dataset for analysis.

3. **Exploratory Data Analysis (EDA)**
   Examining correlations between sleep variables and stress levels.

4. **Modeling**

   * Simple linear regression
   * Multivariate linear regression

The emphasis is on **interpretability** rather than predictive complexity.

---

## Key Findings

* Sleep quality shows a **strong negative relationship** with stress levels.
* Sleep duration shows a **much weaker relationship** with stress when sleep quality is controlled.

### Multivariate Regression Results (Conceptual)

* Sleep Quality coefficient ≈ **-1.27**
* Sleep Duration coefficient ≈ **-0.10**

These results align with **cognitive load theory**: it is not merely how long one sleeps, but whether sleep restores cognitive efficiency.

---

## Theoretical Interpretation

Drawing from cognitive psychology:

* Poor sleep quality increases **extraneous cognitive load**
* Working memory becomes inefficient
* Attention fragments
* Emotional regulation weakens

This cognitive overload is experienced subjectively as **stress**, explaining why sleep quality dominates sleep duration in predicting outcomes.

---

## HCI / Design Implications

From a human centered computing perspective:

* Interfaces should minimize unnecessary cognitive load
* Poor information hierarchy and multitasking-heavy designs may exacerbate stress, especially under sleep deprivation
* Technology can be designed to *support* cognition rather than overload it

---

## Project Structure

```
Behavior-analysis-project/
│
├── data/
│   ├── raw/
│   │   └── sleep_health_lifestyle.csv
│   └── processed/
│       └── sleep_cleaned.csv
│
├── docs/
│   ├── psychology_intro.md
│   ├── working_memory_sleep.md
│   ├── cognitive_load_and_stress.md
│   ├── dataset_description.md
│   ├── data_inspection.md
│   ├── data_cleaning_notes.md
│   ├── mood_operationalization.md
│   └── final_conclusion.md
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_eda_sleep_mood.ipynb
│   ├── 03_modeling.ipynb
│   └── 04_multivariate_regression.ipynb
│
└── README.md
```

---

## Limitations

* Use of self reported data
* Stress used as a proxy for mood
* Cross sectional dataset (no causal inference)

These limitations are acknowledged explicitly to maintain research transparency.

---

## Skills Demonstrated

* Cognitive psychology foundations
* Research style documentation
* Data cleaning and EDA
* Interpretable machine learning
* Theory driven analysis

---

## Future Directions

* Incorporating objective sleep measures (e.g., wearable data)
* Extending analysis to attention or memory performance tasks
* Designing and evaluating cognitively efficient interfaces (HCI focus)

---

## Author Intent

This project was built as part of a long-term academic trajectory toward **Cognitive Science / HCI graduate study**, emphasizing clarity, theory, and research thinking over model complexity.
