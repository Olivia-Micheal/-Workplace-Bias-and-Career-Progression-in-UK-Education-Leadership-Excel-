# Workplace Bias & Career Progression in UK Education Leadership
### Statistical Analysis Using ANOVA | Microsoft Excel | Interactive Dashboard

---

Most people assume experience is the strongest driver of career growth.

This project proved otherwise.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Tools & Skills](#tools--skills)
3. [Dataset](#dataset)
4. [Process Summary](#process-summary)
5. [ANOVA Results](#anova-results)
6. [Key Findings](#key-findings)
7. [Conclusion](#conclusion)
8. [Recommendations](#recommendations)
9. [Author & Contact](#author--contact)
10. [Download Project Files](#download-project-files)

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

> **[INSERT IMAGE HERE — Screenshot of your raw questionnaire data before any cleaning. This shows the messy text responses Excel could not calculate]**
> *Figure 1: Raw questionnaire dataset as received*

---

## Process Summary

**Step 1: Data Coding**

The raw dataset contained text responses that Excel could not calculate. Every column was converted into numerical values using Find and Replace. A coding reference sheet was created and maintained throughout the process to ensure consistency.

| Column | Text Value | Coded Value |
|---|---|---|
| Gender | Female | 1 |
| Gender | Male | 2 |
| Bias Response | Not at all concerned | 1 |
| Bias Response | Slightly concerned | 2 |
| Bias Response | Moderately concerned | 3 |
| Bias Response | Somewhat concerned | 4 |
| Bias Response | Very concerned | 5 |
| Career Behaviour | No / Does not apply | 0 |
| Career Behaviour | Yes / Sometimes | 1 |
| Environment | Not important | 1 |
| Environment | Slightly important | 2 |
| Environment | Somewhat important | 3 |
| Environment | Moderately important | 4 |
| Environment | Very important | 5 |

> **[INSERT IMAGE HERE — Screenshot of your Coding Key sheet showing all coded variables and their assigned values]**
> *Figure 2: Coding reference sheet*

---

**Step 2: Composite Scores**

Three composite scores were created by summing related columns for each respondent. These scores became the core variables used in all five ANOVA tests.

- **PB (Perceived Bias)** - total score from all bias concern columns. Measures how much bias each person felt at work.
- **PPE (Perceived Professional Environment)** - total score from all importance columns. Measures how each person valued their work environment.
- **CP (Career Progression)** - total score from all career behaviour columns. Measures how much each person changed their behaviour just to advance in their career.

> **[INSERT IMAGE HERE — Screenshot of your clean Summary sheet showing Gender, Age, Experience, PB, PPE and CP columns with all 35 rows of data]**
> *Figure 3: Clean summary sheet with composite scores*

---

**Step 3: ANOVA Testing**

ANOVA Single Factor was run five times in Microsoft Excel using the Data Analysis ToolPak - once per hypothesis - at a significance level of **0.05.**

A result is significant when both conditions are met:
- **F value > F critical value**
- **P value < 0.05**

If both conditions are met - the difference between groups is real, not random. If not - no significant difference was found.

---

## ANOVA Results

| Hypothesis | Comparison | F Value | P Value | F Critical | Result |
|---|---|---|---|---|---|
| H1 | Gender vs Perceived Bias | 482.69 | 1.34E-32 | 3.98 | ✅ Significant |
| H2 | Age vs Perceived Bias | 334.75 | 9.26E-28 | 3.98 | ✅ Significant |
| H3 | Experience vs Career Progression | 1.08 | 0.303 | 3.98 | ❌ Not Significant |
| H4 | Gender vs Career Progression | 7.15 | 0.009 | 3.98 | ✅ Significant |
| H5 | Demographics vs Professional Environment | 375.03 | 2.22E-29 | 3.98 | ✅ Significant |

> **[INSERT IMAGE HERE — Screenshot of your H4 ANOVA output showing Gender vs Career Progression. This is your strongest and most surprising finding]**
> *Figure 4: ANOVA output for H4 - Gender vs Career Progression*

---

## Key Findings

**4 out of 5 hypotheses returned statistically significant results.**

Here is what the data actually showed:

- **Gender affects bias perception (H1):** Both males and females experience workplace bias. Males reported slightly higher bias scores (20.4) than females (20.0). The difference is statistically real - not random.

- **Age affects bias perception (H2):** The younger you are, the more workplace bias you feel. Leaders aged 35-39 reported the highest bias score of 26.00. As leaders got older and more senior, their bias scores dropped steadily. Bias hits hardest at the beginning of a career.

- **Experience does NOT affect career progression (H3):** This was the most surprising finding. Holding more administrative roles did not lead to better career outcomes. The result was not statistically significant - meaning the difference between experience levels was essentially random noise.

- **Gender affects career progression (H4):** Female leaders recorded an average career progression score of 10.2 compared to just 1.88 for males. That means females are changing how they look, speak, dress and carry themselves almost **5 times more than males** just to move forward in their careers.

- **Demographics affect professional environment perception (H5):** Males rated their professional environment higher (16.52) than females (15.9). The same workplace feels like a completely different place depending on your gender.

---

## Conclusion

Going into this project, the assumption was straightforward - the more experience a leader has, the further they progress in their career. That is what most people believe. That is what the data was expected to confirm.

It did not.

Experience had no statistically significant relationship with career progression in UK education leadership. What drove career outcomes was not how many roles someone had held. It was who they are.

Gender emerged as the most powerful factor across the entire analysis. Female leaders are not just facing higher levels of behavioural pressure to advance - they are operating in a professional environment that feels fundamentally different from the one their male counterparts experience. The bias is real. The inequality is measurable. And it shows up clearly in the numbers.

Younger leaders feel it the most. As leaders age and gain seniority, bias perception decreases - but it does not disappear. The data suggests that the early stages of a leadership career are where bias does the most damage.

Four out of five hypotheses confirmed what many education leaders have experienced but rarely seen backed by data - that gender shapes both how bias is felt and how careers unfold in UK education leadership. This is not opinion. It is statistical evidence.

---

## Recommendations

1. **Implement unconscious bias training** for all staff involved in hiring and promotion decisions
2. **Introduce mentorship programmes** specifically targeting younger leaders aged 35-39
3. **Review promotion criteria** to ensure transparency and fairness regardless of gender
4. **Conduct regular workplace environment assessments** to improve the experience of female leaders

---

## Author & Contact

**[Olivia Anetoh](https://www.linkedin.com/in/olivia-anetoh-955b94328)**

Data Analyst focused on turning raw, unstructured data into clear business insights.

- LinkedIn: [Olivia Anetoh](https://www.linkedin.com/in/olivia-anetoh-955b94328)
- GitHub: [Olivia-Micheal](https://github.com/Olivia-Micheal)
- Email: anetohchinecherem@gmail.com

---

## Download Project Files

You can access the full project files used in this analysis below.

- [View Excel File - Dashboard & ANOVA Results](https://docs.google.com/spreadsheets/d/16-uxDERNP4HS6xtiPss-8XE9XZx5srWo/edit?usp=drivesdk&ouid=111577166428921651968&rtpof=true&sd=true)
- [View Written Report](https://docs.google.com/document/d/1UQHvDRUCDnTpaawhWmNiEwB_ghUIJ-az/edit?usp=drivesdk&ouid=111577166428921651968&rtpof=true&sd=true)

> **[INSERT IMAGE HERE - Full dashboard screenshot showing all 35 respondents unfiltered]**
> *Figure 5: Full interactive dashboard - all respondents*

> **[INSERT IMAGE HERE - Dashboard filtered to Female respondents, 10 respondents]**
> *Figure 6: Dashboard filtered to Female respondents (10)*

> **[INSERT IMAGE HERE - Dashboard filtered to Male respondents, 25 respondents]**
> *Figure 7: Dashboard filtered to Male respondents (25)*

*Note: Excel file opens in Google Sheets. For best experience, download and open in Microsoft Excel.*

---

*Analyzed by [Olivia Anetoh](https://www.linkedin.com/in/olivia-anetoh-955b94328) - Data Analyst*
