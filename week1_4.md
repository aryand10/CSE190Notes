# Fair Machine Guidance to Enhance Fair Decision Making in Biased People

### Authors:
- **Mingzhe Yang** (University of Tokyo)
- **Hiromi Arai** (RIKEN)
- **Naomi Yamashita** (Kyoto University)
- **Yukino Baba** (University of Tokyo)

Published in CHI '24, May 11-16, 2024, Honolulu, HI, USA.  
DOI: [10.1145/3613904.3642627](https://doi.org/10.1145/3613904.3642627)

---

## Abstract
This study focuses on developing and evaluating an AI system aimed at educating individuals to make unbiased decisions using fairness-aware machine learning. The research involved 99 participants in a between-subjects experimental design, where they were divided into two groups: one receiving AI guidance for fair decision-making and another informed of their biases but without guidance. The study found that fair machine guidance prompted participants to reassess their views on fairness and adjust their decision-making criteria.

---

## Introduction

Human decision-making can often be biased based on attributes like race or gender. This study aims to address such biases through **Fair Machine Guidance**, an AI-driven method to help individuals make more fair decisions by guiding them through a structured learning process. Unlike traditional methods focused solely on raising awareness of biases, this approach actively assists participants in adjusting their decision-making behaviors.

### Key Motivations:
- Raising awareness of biases alone has shown limited effectiveness.
- Fair Machine Guidance seeks to provide actionable guidance to mitigate biases in decision-making.
- The system is based on **fairness-aware machine learning**, which adjusts AI models to ensure fairness.

---

## Research Questions

1. **RQ1**: How does fair machine guidance affect users' motivation to correct bias?
2. **RQ2**: How does fair machine guidance affect users' awareness of the magnitude and direction of bias?
3. **RQ3**: How does fair machine guidance influence users' decision-making criteria?

---

## Methodology

### Fair Machine Guidance System

1. **Student Model**: Captures users' initial decision-making criteria through logistic regression.
2. **Teacher Model**: A fair, machine-learned version of the user’s decision model, adjusted using fairness-aware ML techniques.
3. **Interactive Feedback**: Users are presented with personalized decision-making feedback, comparing their initial (biased) decisions with AI-generated fair decisions.

### Fairness Metric

The fairness-aware model uses **Demographic Parity**, ensuring decisions (e.g., income predictions, credit risk assessments) are independent of sensitive attributes like race or gender.

### Experimental Design

- **Participants**: 99 individuals screened for biased judgments.
- **Tasks**: Participants completed two tasks—predicting **income** (using the Adult dataset) and assessing **credit risk** (using the German Credit dataset).
- **Groups**: Divided into two groups: one receiving only bias feedback, and the other receiving fair machine guidance.
  
---

## Key Results

### 1. **Motivation to Correct Biases (RQ1)**:
   - Participants in the fair machine guidance group were significantly more motivated to reconsider fairness compared to those who received only bias feedback.
   - Several participants recognized their own unconscious biases through AI feedback and adjusted their decision-making behavior accordingly.

   **Example Participant Feedback**:
   - "I thought I was being fair, but the AI showed me otherwise." 
   - Participants who received AI guidance were more likely to accept societal expectations of fairness.

### 2. **Awareness of Bias Direction and Magnitude (RQ2)**:
   - Fair machine guidance significantly increased awareness of the specific decision criteria participants were using to make biased decisions (e.g., race or occupation).
   - Participants reflected more critically on their judgments, leading to a deeper understanding of how they made biased decisions.

   **Example Feedback**:
   - "I realized I was judging too heavily based on education background."
   - Bias feedback alone did not prompt the same level of critical reflection.

### 3. **Adjustment of Decision Criteria (RQ3)**:
   - Fair machine guidance led to statistically significant changes in decision-making criteria. Participants who received this guidance were more likely to modify their decision-making processes.
   - Many accepted AI-generated advice after carefully considering the suggestions, even when it differed from their initial judgment.
   
   **Examples**:
   - "The AI showed me new factors I should consider in decision-making."
   - However, 11 participants did not change their criteria, often due to mistrust or discomfort with AI advice.

---

## Discussion

### Fair Machine Guidance vs. Bias Feedback
- **Fair machine guidance** was more effective than bias feedback in prompting users to reconsider and adjust their decision-making processes.
- Participants found fair machine guidance more helpful for reflecting on fairness and adjusting their criteria for more equitable decisions.

### Algorithmic Aversion
- Some participants exhibited skepticism towards AI-driven guidance, a phenomenon known as **algorithmic aversion**.
- Participants questioned the AI’s fairness in some cases, particularly when its suggestions conflicted with their personal views on fairness.

---

## Conclusion

The study shows that fair machine guidance is a promising tool for mitigating biased decision-making. By guiding users through a structured learning process, the AI system helped participants become more aware of their biases and adjust their decision criteria. The findings suggest that AI systems can play a critical role in teaching fair decision-making, but it is crucial to address challenges like algorithmic aversion to maximize their impact.

---

## References

1. "Fairness-aware machine learning" [Source]
2. "Demographic Parity" [Source]
