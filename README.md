# Workplace Bias & Career Progression in UK Education Leadership
### Statistical Analysis Using ANOVA | Microsoft Excel | Interactive Dashboard

---

Most people assume experience is the strongest driver of career growth.

This project proved otherwise.

---

## Project Overview

This project involved analyzing a **raw questionnaire survey** completed by **35 education leaders in the United Kingdom**. The goal was to determine whether demographic factors such as **gender, age, and experience** influence how workplace bias is perceived and how careers progress in UK education leadership.

The dataset arrived as unstructured text responses. Before any analysis could begin, the data had to be cleaned, coded, and transformed into a format suitable for statistical testing.

**Business Problem:** Does workplace bias exist in UK education leadership, and does it affect people differently based on who they are?

---

## Tools & Skills

| Tool | Purpose |
|---|---|
| Microsoft Excel | Data cleaning, coding, analysis, dashboard |
| Data Analysis ToolPak | ANOVA Single Factor testing |
| Pivot Tables & Charts | Dashboard visualisation |
| Microsoft Word | Written report |

**Skills Demonstrated:**
Data Coding | Data Cleaning | Composite Score Creation | ANOVA | Hypothesis Testing | Dashboard Design | Data Storytelling | Report Writing

---

## Dataset

- **Source:** Structured questionnaire survey
- **Respondents:** 35 UK education leaders (superintendents)
- **Format:** Raw text responses across multiple columns
- **Topics covered:** Demographics, workplace bias perception, career progression behaviour, professional environment assessment

> **[ADD IMAGE HERE — Screenshot of raw questionnaire data before any cleaning]**
> *Figure 1: Raw questionnaire dataset as received*

---

## Process Summary

**Step 1: Data Coding**

All text responses were converted to numerical values using Find and Replace in Excel. A coding reference sheet was maintained throughout.

| Column | Text Value | Coded Value |
|---|---|---|
| Gender | Female | 1 |
| Gender | Male | 2 |
| Bias Response | Not at all concerned | 1 |
| Bias Response | Very concerned | 5 |
| Career Behaviour | No / Does not apply | 0 |
| Career Behaviour | Yes / Sometimes | 1 |
| Environment | Not important | 1 |
| Environment | Very important | 5 |

> **[ADD IMAGE HERE — Screenshot of your Coding Key sheet]**
> *Figure 2: Coding reference sheet showing all coded variables*

---

**Step 2: Composite Scores**

Three scores were created by summing related columns for each respondent:

- **PB (Perceived Bias)** - total score from all bias concern columns
- **PPE (Perceived Professional Environment)** - total score from all importance columns
- **CP (Career Progression)** - total score from all career behaviour columns

> **[ADD IMAGE HERE — Screenshot of your clean Summary sheet showing Gender, Age, Experience, PB, PPE, CP columns]**
> *Figure 3: Clean summary sheet with composite scores*

---

**Step 3: ANOVA Testing**

ANOVA Single Factor was run five times - once per hypothesis - at a **significance level of 0.05.**

A result is significant when:
- **F value > F critical** AND
- **P value < 0.05**

---

## ANOVA Results

| Hypothesis | Comparison | F Value | P Value | F Critical | Result |
|---|---|---|---|---|---|
| H1 | Gender vs Bias | 482.69 | 1.34E-32 | 3.98 | ✅ Significant |
| H2 | Age vs Bias | 334.75 | 9.26E-28 | 3.98 | ✅ Significant |
| H3 | Experience vs Career Progression | 1.08 | 0.303 | 3.98 | ❌ Not Significant |
| H4 | Gender vs Career Progression | 7.15 | 0.009 | 3.98 | ✅ Significant |
| H5 | Demographics vs Environment | 375.03 | 2.22E-29 | 3.98 | ✅ Significant |

> **[ADD IMAGE HERE — Screenshot of your H4 ANOVA output. Gender vs Career Progression. This is your most powerful finding]**
> *Figure 4: ANOVA output for H4 - Gender vs Career Progression*

---

## Key Findings

- **4 out of 5 hypotheses** returned statistically significant results
- **Younger leaders (35-39)** reported the highest workplace bias scores (26.00), declining steadily with age
- **Female leaders** showed nearly **5x higher** career behavioural adaptation scores than males (10.2 vs 1.88) - changing how they look, speak and present themselves just to advance
- **Males rated their professional environment higher** (16.52) than females (15.9) - the same workplace feels different depending on your gender
- **Experience showed no significant relationship with career progression** - the most surprising finding of the entire project

---

## Dashboard

> **[ADD IMAGE HERE — Full dashboard screenshot, all 35 respondents unfiltered]**
> *Figure 5: Full interactive dashboard showing all 35 respondents*

> **[ADD IMAGE HERE — Dashboard filtered to Female, 10 respondents]**
> *Figure 6: Dashboard filtered to Female respondents (10)*

> **[ADD IMAGE HERE — Dashboard filtered to Male, 25 respondents]**
> *Figure 7: Dashboard filtered to Male respondents (25)*

**Dashboard features:**
- 5 interactive bar charts - one per hypothesis
- 3 dynamic KPIs - Total Respondents, Hypotheses Tested, Significant Findings
- 2 slicers - Gender and Age
- Navigation panel with links to raw data and ANOVA results

---

## Recommendations

1. **Implement unconscious bias training** for all staff involved in hiring and promotion decisions
2. **Introduce mentorship programmes** specifically targeting younger leaders aged 35-39
3. **Review promotion criteria** to ensure transparency and fairness regardless of gender
4. **Conduct regular workplace environment assessments** to improve the experience of female leaders

---

## Repository Structure
