# A Framework for Understanding Sources of Harm Throughout the Machine Learning Life Cycle

### Authors:
- **Harini Suresh** (MIT)
- **John Guttag** (MIT)

Published in EAAMO '21, October 5-9, 2021.  
DOI: [10.1145/3465416.3483305](https://doi.org/10.1145/3465416.3483305)

---

## Abstract
As Machine Learning (ML) becomes more pervasive in society, understanding the sources of harm that can be introduced across the ML lifecycle is crucial. The paper presents a framework that identifies seven distinct sources of potential downstream harm, spanning the stages of data collection, development, and deployment. It aims to help practitioners better anticipate and address these issues, fostering more transparent and fair ML systems.

---

## Key Terminology
- **Allocative Harm**: Denial of opportunities or resources to certain groups.
- **Representational Harm**: The reinforcement of harmful stereotypes or stigma through ML models.

---

## Introduction

ML impacts critical decisions in various fields, including facial analysis and criminal justice systems, with potential for harm due to biased models and data. This paper explores how each stage of the ML lifecycle can contribute to such harm and provides a structured way to understand and mitigate these risks.

Common misconceptions such as "data is biased" oversimplify the issue, neglecting the complexity of how bias enters the ML lifecycle through human decisions and historical contexts.

---

## Machine Learning Overview

### ML Lifecycle Stages:
1. **Data Collection**: Involves identifying the target population and features. Harm can arise if the sampled data is unrepresentative.
2. **Data Preparation**: Preprocessing steps (like normalization or dealing with missing data) can introduce bias.
3. **Model Development**: Models are trained and optimized, often reinforcing biases present in the data.
4. **Model Evaluation**: Typically performed on benchmark datasets, which may not represent real-world populations.
5. **Model Postprocessing**: Adjustments like setting thresholds can impact how model outcomes are presented.
6. **Model Deployment**: The real-world use of models often deviates from the controlled environments they were developed in, leading to unforeseen consequences.

---

## Seven Sources of Harm in Machine Learning

### 1. **Historical Bias**
   - Even with perfectly measured and sampled data, historical inequalities or societal biases can be reflected in ML outcomes.
   - **Example**: Word embeddings that associate gender stereotypes with occupations based on historical data.

### 2. **Representation Bias**
   - Occurs when the development sample under-represents certain populations, leading to poor generalization.
   - **Example**: ImageNet disproportionately represents Western countries, leading to worse performance in images from underrepresented regions.

### 3. **Measurement Bias**
   - Happens when the features and labels used in ML do not accurately capture the desired constructs, often varying across different groups.
   - **Example**: Risk assessment tools in the criminal justice system use “arrest” as a proxy for crime, misrepresenting risk for minority communities.

### 4. **Aggregation Bias**
   - Using a single model for diverse groups can fail to account for differences between them, leading to suboptimal performance for all or some groups.
   - **Example**: A generalized sentiment analysis model might misinterpret culturally specific slang or terms, leading to harmful misclassifications.

### 5. **Learning Bias**
   - Choices made during model optimization (such as focusing on accuracy) can amplify disparities across groups.
   - **Example**: Optimizing for privacy or compactness can worsen performance on underrepresented groups.

### 6. **Evaluation Bias**
   - Occurs when benchmark datasets used to evaluate models are not representative of the intended use population.
   - **Example**: Commercial facial recognition systems performing poorly on dark-skinned women due to lack of representation in the benchmark datasets.

### 7. **Deployment Bias**
   - Arises when the real-world use of a model differs from the environment it was designed and evaluated in, leading to harm.
   - **Example**: Risk assessment tools being used for sentencing, despite being designed for pretrial decisions.

---

## Mitigation Strategies

The paper suggests that understanding the specific sources of harm can help in designing more targeted mitigations, such as:

- **Improving data collection and measurement** to capture the complexities of real-world situations.
- **Tailoring models** to different subgroups or using multitask learning to address aggregation bias.
- **Evaluating models on more representative datasets** or using broader performance metrics.

Mitigation efforts should consider application-specific needs, as fairness is not a one-size-fits-all concept.

---

## Conclusion

This framework helps in structuring discussions around fairness and harm in ML by pinpointing specific sources of bias throughout the ML lifecycle. By focusing on targeted, application-grounded solutions, the framework facilitates more thoughtful and effective mitigation strategies, ensuring that ML systems are more aligned with fairness and societal welfare.

---

## References
- [Barocas et al., 2017] Allocative and representational harms in ML systems.
- [Buolamwini and Gebru, 2018] Gender Shades: Biases in commercial facial analysis systems.
- [Friedman and Nissenbaum, 1996] Pre-existing bias in computer systems.
