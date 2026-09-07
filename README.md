# Workplace Bias and Career Progression in UK Education Leadership (Excel)
A statistical investigation into whether gender, age, and experience shape how UK education leaders experience workplace bias, career progression, and professional environment.

## 📌 Overview / Business Problem
**Central question:** Does workplace bias exist in UK education leadership, and if so, does it affect people differently based on who they are?

This breaks down into five testable questions:
1. Does perceived workplace bias differ significantly across gender groups?
2. Does perceived workplace bias differ significantly across age groups?
3. Does professional experience significantly influence career progression?
4. Does gender significantly influence career progression?
5. Does perception of the professional environment differ significantly across demographic groups?

**Who would act on this:** HR/DEI leads and senior leadership in education institutions deciding where to target bias-reduction and mentorship investment.

---

## 📊 Dataset
- Source: questionnaire collected from **35 education leaders (superintendents)** in the UK
- Format: survey responses — demographic fields (gender, age, experience) plus Likert-scale questions on bias, career behaviour, and professional environment
- Raw responses were text-based (e.g. "Slightly", "Moderately"), not analyzable in that form — see Methodology for how this was handled

*[IMAGE: raw dataset screenshot — a few rows showing the original text-based survey columns]*

---

## 🛠️ Tools & Technologies
- **Microsoft Excel** — data cleaning, coding, ANOVA analysis, dashboard
- **Data Analysis ToolPak** — ANOVA Single Factor testing
- **Pivot Tables & Pivot Charts** — dashboard visualisation
- **Microsoft Word** — written report

---

## 🔍 Methodology
**Step 1 — Data coding:** Raw text responses couldn't be calculated in Excel, so every column was numerically coded using Find and Replace (e.g. Gender: Female=1, Male=2; Bias concern: Not at all=1 → Very=5). A coding key reference sheet was maintained throughout to keep the mapping auditable.

*[IMAGE: coding key reference sheet]*

**Step 2 — Composite scores:** Related columns were summed into three composite scores per respondent, since no single survey question could represent bias, environment, or progression on its own:
- **PB** (Perceived Bias) — sum of all "how concerned were you" columns
- **PPE** (Perceived Professional Environment) — sum of all "how important were the following" columns
- **CP** (Career Progression) — sum of all "have you ever intentionally" columns

**Step 3 — Summary sheet:** A clean sheet was built with only the six columns needed for analysis (Gender, Age, Experience, PB, PPE, CP) — isolating signal from the full raw survey before running any test.

**Step 4 — ANOVA testing:** ANOVA Single Factor was run once per hypothesis (5 runs total) via the Data Analysis ToolPak, at a 0.05 significance level. Each result was read using three values together — F, F critical, and P — rather than any one number alone:
- F > F critical **and** P < 0.05 → significant, reject null hypothesis
- F < F critical **and** P > 0.05 → not significant, retain null hypothesis

---

## 🖥️ Dashboard Walkthrough
*[IMAGE: full dashboard overview screenshot]*

**KPI panel** — Total Respondents (dynamic count), Hypotheses Tested (5), Significant Findings (4 of 5). Built to give a viewer the headline result in the first three seconds, before they read a single chart.

*[IMAGE: KPI panel close-up]*

**Five bar charts, one per hypothesis** — each chart carries an insight line directly under its title connecting the visual back to the research question it answers, so the chart never needs a separate caption to be understood.

*[IMAGE: chart — Gender vs Perceived Bias]*
*[IMAGE: chart — Age vs Perceived Bias]*
*[IMAGE: chart — Experience vs Career Progression]*
*[IMAGE: chart — Gender vs Career Progression]*
*[IMAGE: chart — Demographics vs Professional Environment]*

**Slicers (Gender, Age)** — connected to all five charts, letting a viewer filter the whole dashboard by demographic group interactively rather than reading static splits.

*[IMAGE: slicers in use, filtered view]*

**Navigation panel** — left-side links to the ANOVA results sheet, raw data sheet, and LinkedIn profile, so a reviewer can move from summary to raw evidence without hunting through tabs.

---

## 💡 Key Findings
- **Gender → Bias:** Significant difference (F=482.69, F crit=3.98, P=1.34E-32). Males scored slightly higher (20.4) than females (20.0) — both groups experience workplace bias, but not equally.
- **Age → Bias:** Significant difference (F=334.75, F crit=3.98, P=9.26E-28). Leaders aged 35–39 reported the highest bias score (26.00); perception decreases steadily with age — younger professionals feel bias most acutely.
- **Experience → Career Progression:** Not significant (F=1.08, F crit=3.98, P=0.303) — the only hypothesis that failed. Holding more administrative roles doesn't guarantee better career outcomes, challenging the assumption that experience alone drives progression.
- **Gender → Career Progression:** Significant difference (F=7.15, F crit=3.98, P=0.009). Female leaders recorded a CP score of 10.2 vs 1.88 for males — women are modifying their behaviour roughly 5x more than men just to advance.
- **Demographics → Professional Environment:** Significant difference (F=375.03, F crit=3.98, P=2.22E-29). Males rated their environment higher (16.52) than females (15.9) — the same workplace is not experienced equally.

**Bottom line:** 4 of 5 hypotheses were statistically significant. Gender is the strongest factor shaping both bias perception and career progression in UK education leadership.

---

## ✅ Recommendations
1. Implement mandatory unconscious bias training for all staff involved in hiring and promotion — directly targets the gender and age bias findings above.
2. Introduce mentorship programmes specifically for leaders aged 35–39 — this group reported the highest bias score.
3. Review promotion criteria for fairness and transparency regardless of gender — addresses the 5x behaviour-modification gap found in career progression.
4. Conduct regular workplace environment assessments focused on the female leader experience — the environment finding shows the same workplace isn't perceived equally.

---

## 📁 Repository Structure
