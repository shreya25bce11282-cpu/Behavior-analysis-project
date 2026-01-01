# Mediation Analysis: Sleep Quality as a Cognitive Mechanism

This analysis investigates whether **sleep quality mediates the relationship between sleep duration and stress levels**, rather than sleep duration directly influencing stress.

This framing aligns with cognitive science perspectives that emphasize **subjective experience as a mediating layer** between physiological states and affective outcomes.


## Conceptual Motivation
Cognitive science research emphasizes that subjective experience often mediates the impact of objective physiological conditions on affective outcomes. In the context of sleep, duration represents an objective measure, whereas sleep quality reflects internal cognitive appraisal.

This analysis tests whether subjective sleep quality mediates the relationship between sleep duration and stress levels.

---

## Model Specification

- **Predictor (X):** Sleep Hours  
- **Mediator (M):** Sleep Quality  
- **Outcome (Y):** Stress Level  

A three-step regression-based mediation approach was used.

---

## Results

### Path A: Sleep Duration → Sleep Quality
An OLS regression showed that sleep duration significantly predicts subjective sleep quality:

- **β = 1.33**, *p* < 0.001  
- **R² = 0.78**

This indicates that objective sleep duration explains a substantial portion of variance in subjective sleep experience.

---

### Path B: Sleep Quality → Stress Level
Sleep quality was a strong negative predictor of stress levels:

- **β = −1.23**, *p* < 0.001

Higher perceived sleep quality was associated with significantly lower stress.

---

### Path C′: Sleep Duration → Stress Level (Controlling for Sleep Quality)
When sleep quality was included in the model, sleep duration was no longer a significant predictor of stress (*p* > 0.05), while sleep quality remained significant.

---

## Interpretation
These results indicate **full mediation**, suggesting that the effect of sleep duration on stress operates primarily through subjective sleep quality rather than directly.

This supports cognitive models in which internal appraisal and perception mediate the relationship between objective conditions and affective outcomes.

---

## Cognitive Science Relevance
The findings operationalize a core cognitive science principle: **internal representations and subjective experience mediate the influence of physical inputs on psychological states**. This mediation framework bridges behavioral data with cognitive theory, highlighting the role of perception and appraisal in stress regulation.

---

## Cognitive Science Interpretation

These results support a mediation framework in which **sleep quality functions as a cognitive-affective mediator**.

Rather than sleep duration directly reducing stress, longer sleep appears to reduce stress primarily by improving subjective sleep quality. This aligns with cognitive theories of:

- Cognitive load reduction
- Improved working memory efficiency
- Enhanced emotional regulation

In this framework, stress is not a direct consequence of biological sleep length, but an experiential outcome shaped by perceived cognitive restoration.


