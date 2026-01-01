# Behavior Analysis Project

## Overview

This project explores the relationship between **sleep, cognition, and mood-related outcomes** using a combination of **cognitive psychology theory** and **interpretable machine learning models**. 

Rather than treating machine learning as a black box, this project is **theory driven**: concepts from attention, working memory, and cognitive load guide the choice of variables, analysis, and interpretation of results.

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
* Nature: Self reported measures

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
   Understanding variable distributions and potential limitations of self-reported data.

2. **Data Cleaning**
   Selecting relevant variables and producing a cleaned dataset for analysis.

3. **Exploratory Data Analysis (EDA)**
   Examining correlations between sleep variables and stress levels.

4. **Modeling**

   * Simple linear regression
   * Multivariate linear regression

The emphasis is on **interpretability** rather than predictive complexity.

---
##  Tech Stack
- **Python**
- Pandas
- Matplotlib / Seaborn
- Jupyter Notebook

### Key Findings
- Sleep quality shows a strong negative relationship with stress levels.
- Sleep duration shows a much weaker relationship with stress once sleep quality is controlled.

Mediation analysis indicates that **sleep quality mediates the relationship between sleep duration and stress**, suggesting that subjective cognitive restoration — not sleep length alone — drives stress regulation.

→ Detailed analysis: [`docs/mediation_sleep_quality.md`](docs/mediation_sleep_quality.md)
.

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
│   ├── mediation_sleep_quality.md
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

## Project Significance
This project represents the **behavioural analysis phase** of a larger human centred research pipeline:

- **Project 1:** Behavioural understanding through psychological data analysis *(this project)*
- **Project 2:** Cognitive load and stress — theoretical analysis  
- **Project 3:** Predicting cognitive fatigue from digital interaction patterns (computational modeling)


Together, these projects aim to bridge **psychology, data science, and human–computer interaction**.

---

## Research Arc

This repository represents one component of a broader research trajectory in Cognitive Science.

A full overview of how this project connects with related theoretical and computational work is documented here:

→ 📄 **Research Arc:** [`docs/research_arc.md`](docs/research_arc.md)

The arc integrates:
- Behavioral data analysis of sleep and stress
- Cognitive theory on load, working memory, and fatigue
- Computational modeling of latent cognitive states from interaction data

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
This work progressively moves from self-reported measures toward passive behavioral inference of cognitive states, aligning with modern directions in computational cognitive science and HCI.

---

## Author Intent

This project was built as part of a long term academic trajectory toward Cognitive Science / HCI graduate study, emphasizing **mechanistic explanation, mediation based reasoning, and theory driven analysis** over model complexity.


---

## 📄 Author
**Shreya Adhikary**  
B.Tech Computer Science  
Psychology + Technology | Behavioural Data Analysis

---
