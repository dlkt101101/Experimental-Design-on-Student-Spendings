# Budget Beliefs: Testing Bias in Perceived Spending Habits

An experimental design and statistical analysis project investigating how student spending allocations are influenced by budget constraints and gender perception. Completed as part of **STAT 332: Sampling and Experimental Design** at the University of Waterloo by Madison, Raymond, and Darren.

---

## 📋 Table of Contents
1. [Overview](#-overview)
2. [Experimental Design](#-experimental-design)
3. [Data & Variables](#-data--variables)
4. [Exploratory Analysis & Results](#-exploratory-analysis--results)
5. [Key Findings & Conclusions](#-key-findings--conclusions)
6. [Limitations & Future Extensions](#-limitations--future-extensions)

---

## 🔍 Overview

How do people perceive student spending, and do implicit biases affect how financial responsibilities are judged? This project explores whether participants allocate funds differently between essentials and non-essentials based on:
* **Budget Level:** Minimum ($1,050), Average ($1,700), and Maximum ($2,200) monthly budgets[cite: 1].
* **Gender Perception:** Whether the allocated budget target is perceived as male or female (e.g., Christopher vs. Sara/Madison)[cite: 1].

**Why it matters:** Understanding these financial biases helps uncover stereotypical spending assumptions (akin to real-world phenomena like the "Pink Tax") before they shape broader economic decisions[cite: 1].

---

## 🧪 Experimental Design

We utilized a **$2 \times 3$ Factorial Design** with a **blocking variable** on the gender of the participant[cite: 1].

* **Factor 1 (Budget Level):** 3 levels (Low: $1,050, Medium: $1,700, High: $2,200)[cite: 1].
* **Factor 2 (Gender Perception):** 2 levels (Male vs. Female name assigned to the budget profile)[cite: 1].
* **Blocking Variable:** Participant Gender (Male vs. Female)[cite: 1].
* **Sample Size:** 60 participants total, with 10 participants (5 male, 5 female) assigned to each of the 6 treatment versions[cite: 1].
* **Response Variable:** Proportion of total budget allocated to essential items (e.g., rent, groceries, healthcare vs. takeout, subscriptions, shopping)[cite: 1].

---

## 📊 Data & Variables

The collected dataset consists of responses structured around monthly budget templates where participants distributed funds across typical undergraduate expense categories:

| Column / Variable | Type | Description |
| :--- | :--- | :--- |
| **ID** | Identifier | Unique participant ID (1 to 60)[cite: 1] |
| **Gender of Participant** | Blocking Variable | Gender of the person filling out the survey[cite: 1] |
| **Budget Level** | Factor 1 | Target monthly budget constraint ($1,050, $1,700, $2,200)[cite: 1] |
| **Gender of Name** | Factor 2 | Perceived gender of the student profile (Male/Female)[cite: 1] |
| **% Spent on Essentials** | Response Variable ($Y$) | The proportion of the total budget allocated to essential categories[cite: 1] |

---

## 📈 Exploratory Analysis & Results

Data analysis was conducted using **R**, utilizing Analysis of Variance (ANOVA) and interaction plots to evaluate main effects and interactions at a significance level of $\alpha = 0.05$[cite: 1].

### ANOVA Summary Table
* **Budget Level (Factor 1):** Highly significant ($p < 0.001$), showing a strong main effect where higher budgets lead to a lower proportion allocated to essentials[cite: 1].
* **Gender Perception (Factor 2):** Insignificant main effect ($p \approx 0.140$)[cite: 1].
* **Participant Block:** Insignificant blocking factor ($p \approx 0.544$)[cite: 1].
* **Interaction (Factor 1 $\times$ Factor 2):** Statistically significant interaction ($p = 0.041$), indicating that the effect of budget level on essential allocations depends on the gender perception of the profile[cite: 1].

---

## 💡 Key Findings & Conclusions

1. **Budget Constraints Drive Allocations:** As total monthly budgets increase, participants naturally shift a smaller proportion toward essentials and allocate more flexibility toward non-essentials[cite: 1].
2. **Gender Interaction Bias:** While gender perception alone did not dictate spending allocation across the board, its significant interaction with budget levels highlights subtle biases in how male vs. female student budgets are evaluated at scale[cite: 1].

---

## ⚠️ Limitations & Future Extensions

* **Limitations:** 
  * The blocking factor (`Gender of name`) was statistically insignificant[cite: 1].
  * Relatively small sample size relative to the broader population[cite: 1].
  * Essential vs. non-essential classifications were pre-determined by our team's interpretation rather than letting participants define them independently[cite: 1].
* **Potential Extensions:**
  * Introducing new blocking variables, such as comparing **International vs. Domestic students**[cite: 1].
  * Adding rich contextual vignettes detailing a student's specific living situation to measure how qualitative context alters financial allocations[cite: 1].

---

## 👥 Contributors
* **Madison**[cite: 1]
* **Raymond**[cite: 1]
* **Darren**[cite: 1]
