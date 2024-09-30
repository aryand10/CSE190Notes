# Soliciting Stakeholders’ Fairness Notions in Child Maltreatment Predictive Systems

### Authors:
- **Hao-Fei Cheng** (University of Minnesota)
- **Paige Bullock** (Kenyon College)
- **Logan Stapleton** (University of Minnesota)
- **Alexandra Chouldechova**, **Haiyi Zhu**, **Ruiqi Wang**, **Zhiwei Steven Wu** (Carnegie Mellon University)

Published in CHI '21, May 8-13, 2021.  
DOI: [10.1145/3411764.3445308](https://doi.org/10.1145/3411764.3445308)

---

## Abstract
The study introduces a framework for eliciting fairness perspectives from non-technical stakeholders in the development of child maltreatment predictive systems. By combining an interactive interface with interviews, the authors extract stakeholders’ nuanced viewpoints on fairness and biases. The study evaluates this framework in the context of a child maltreatment risk assessment tool, uncovering preferences for fairness notions like equalized odds and revealing challenges in balancing fairness with predictive accuracy.

---

## Key Terms
- **Algorithmic Fairness**: Ensuring that machine learning systems treat individuals and groups fairly.
- **Equalized Odds**: A fairness criterion where the false positive and false negative rates are equal across sensitive groups (e.g., race, gender).
- **Statistical Parity**: Ensuring that the algorithm predicts equal positive classification rates across groups.
- **Unawareness**: Ignoring sensitive attributes like race or gender in the decision-making process.

---

## Introduction

The increasing reliance on machine learning (ML) in high-stakes areas like child welfare necessitates an understanding of fairness in algorithm-assisted decision-making. Previous research on ML fairness has proposed various group and individual fairness definitions. However, there remains a gap in how these fairness notions align with the perspectives of stakeholders directly affected by these decisions.

The paper proposes a **novel framework** to elicit fairness perspectives from stakeholders in child maltreatment predictive systems. This framework uses an **interactive interface** that allows users to explore algorithmic decisions at both individual and group levels, combined with interviews to probe their fairness viewpoints. The framework is evaluated in the context of the **Allegheny Family Screening Tool (AFST)**, a real-world ML-based risk assessment tool used to assist child abuse hotline workers.

---

## Machine Learning Fairness Approaches

1. **Group Fairness**: Achieving equality across pre-defined demographic groups (e.g., race or gender). Common definitions include:
   - **Unawareness**: Ignoring sensitive attributes during decision-making.
   - **Statistical Parity**: Ensuring that the positive classification rates are equal across groups.
   - **Equalized Odds**: Ensuring equal false positive and false negative rates across groups.

2. **Individual Fairness**: Requiring that "similar individuals be treated similarly." However, defining similarity metrics in real-world scenarios can be difficult.

---

## Framework for Eliciting Fairness from Stakeholders

### Research Question
**How can we effectively elicit fairness notions from non-technical stakeholders in child maltreatment predictive systems?**

### Framework Components:
1. **Interactive Interface**: Enables stakeholders to examine the algorithm’s predictions and compare data at both group and individual levels. The interface consists of three views:
   - **Group View**: Allows users to explore fairness metrics across user-defined groups.
   - **Case-by-Case View**: Facilitates pairwise comparisons of algorithmic decisions for individual cases.
   - **Similarity Comparison View**: Enables stakeholders to compare a reference case with all other cases in the dataset.
   
2. **Interview Protocol**: Probes stakeholders' reasoning about fairness, focusing on their reactions to different fairness definitions and algorithmic outcomes.

---

## User Study Design

The study involved **12 participants** split into two groups:
- **Social workers**: With experience in child abuse investigations.
- **Parents**: Concerned stakeholders affected by the child welfare system.

Participants used the interactive interface to explore synthetic data modeled after the AFST dataset. They were asked to assess fairness using three fairness criteria—**equalized odds**, **statistical parity**, and **unawareness**—across five sensitive attributes (victim age, gender, family race, public assistance usage, perpetrator gender).

---

## Key Results

### Group Fairness Preferences:
- **Equalized Odds** was the most supported fairness criterion, with **66.7%** of participants favoring it.
- **Statistical Parity** was supported by **43.3%**, and **Unawareness** by **41.7%**.
- Participants preferred **equalized odds** because it aligns with their belief that algorithms should be equally accurate across sensitive groups.
- However, they were generally unwilling to sacrifice overall accuracy to achieve this.

### Individual Fairness:
- There was little consensus on individual fairness. For most case pairs presented to participants, no clear majority agreement was reached on how the algorithm should prioritize them.

---

## Discussion

### Fairness Trade-offs:
Participants acknowledged that while **equalized odds** provides a desirable fairness metric, enforcing it may reduce accuracy for certain groups. Some participants preferred to **prioritize accuracy** over strict fairness metrics, especially when dealing with high-risk populations in child welfare cases.

### Context-Specific Fairness:
Participants emphasized that fairness in child welfare should account for **contextual differences** between cases, such as differences in abuse types and victim vulnerability (e.g., younger children being more vulnerable).

---

## Ethical Considerations

The use of algorithmic tools in child welfare, such as the AFST, remains controversial due to concerns about reinforcing historical biases against marginalized communities. While data-driven decision-making has the potential to improve child welfare outcomes, the framework stresses the importance of **involving stakeholders** in the algorithmic design process to ensure fairness and mitigate systemic discrimination.

---

## Conclusion

The framework provides a structured way to solicit fairness perspectives from non-technical stakeholders, offering valuable insights for improving child maltreatment predictive systems. The study demonstrates that involving stakeholders in the fairness evaluation process can lead to a more nuanced understanding of fairness in machine learning, especially in sensitive, high-stakes contexts like child welfare.
