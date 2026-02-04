---
layout: default
title: Project 4 - Method and Results
---

[Back to Project 4](project4.html)

# Method and Results - Project 4

**Title**: The impact of leader workaholism on female working students' reproductive health

**Team**: Quin & Michelle

---

## Method

### Participants

Participants were 86 female working students recruited from a public university in the western United States. Eligibility criteria required that participants be currently employed and enrolled in college courses at the time of the study. Of the 86 participants, 74 had complete data on all study variables and were included in the hypothesis testing analyses.

Participants' average age was 24.36 years (*SD* = 6.90, range = 18–66). The sample was ethnically diverse: 50.0% identified as Latinx, 16.3% as White, 11.6% as Asian, 4.7% as Black or African American, and 17.4% identified with multiple or other racial backgrounds. Regarding education, 46.5% held an associate's degree, 32.6% had a high school diploma or GED, 18.6% had a bachelor's degree, and 1.2% had a master's degree. Participants worked an average of 33.73 hours per week (*SD* = 21.92), had been with their current organization for an average of 6.13 years (*SD* = 9.96), and were enrolled in an average of 14.17 credit hours (*SD* = 2.35). The most common industries represented were health care (12.8%), education (11.6%), administrative services (9.3%), and financial and insurance (7.0%).

### Procedure

Data were collected via an online survey hosted on Qualtrics. Participants were recruited through the university's participant pool. After providing informed consent, participants completed measures assessing their perceptions of their supervisor's workaholism, their own after-hours technology use, and reproductive health symptoms. All procedures were approved by the university's Institutional Review Board.

### Measures

**Leader workaholism (cognitive).** Participants rated their supervisor's cognitive workaholism using four items from the cognitive subscale of the Multidimensional Workaholism Scale (Clark et al., 2020). This subscale captures the extent to which supervisors appear to think compulsively about work. A sample item is "It feels like my supervisor cannot stop themself from thinking about working." Responses were rated on a 5-point scale ranging from 1 (*strongly disagree*) to 5 (*strongly agree*; α = .92).

**After-hours ICT use.** After-hours information and communication technology (ICT) use was assessed with a single item asking participants how often they used work-related ICTs (e.g., email, messaging apps, phone calls) outside of formal work hours in the past week (Boswell & Olson-Buchanan, 2007). Response options ranged from 1 (*never*) to 5 (*almost always*).

**Heavy menstrual bleeding.** Heavy menstrual bleeding (menorrhagia) was assessed with a single item: "Rate the extent to which you experience heavy menstrual bleeding (menorrhagia)." Responses ranged from 1 (*not at all*) to 5 (*extremely*).

### Analytic Strategy

Analyses were conducted using Python 3.13 with the pandas, NumPy, SciPy, and statsmodels libraries. First, we computed descriptive statistics and bivariate correlations among all study variables. Second, we assessed the reliability of the multi-item scale using Cronbach's alpha. Third, we tested hypotheses using ordinary least squares regression. Given the exploratory nature of this study and the relatively small sample size, we evaluated statistical significance at the *p* < .10 level.

---

## Results

### Preliminary Analyses

Means, standard deviations, and correlations among study variables are presented in Table 1. Among demographic variables, age was positively correlated with working hours (*r* = .26, *p* < .05) and organizational tenure (*r* = .54, *p* < .01). Credit hours was marginally positively correlated with after-hours ICT use (*r* = .20, *p* < .10). For the main study variables, leader workaholism (cognitive) was positively correlated with after-hours ICT use (*r* = .23, *p* < .05), and after-hours ICT use was positively correlated with heavy menstrual bleeding (*r* = .23, *p* < .05). Leader workaholism was not significantly correlated with heavy menstrual bleeding (*r* = -.01, *p* = .94).

### Hypothesis Tests

**Hypothesis 1** predicted that leader workaholism (cognitive) would be positively related to employees' after-hours ICT use. Leader workaholism was positively associated with after-hours ICT use (*b* = 0.31, *SE* = 0.16, *p* < .05). Hypothesis 1 was supported.

**Hypothesis 2** predicted that after-hours ICT use would be positively related to heavy menstrual bleeding. After-hours ICT use was positively associated with heavy menstrual bleeding (*b* = 0.16, *SE* = 0.08, *p* < .05). Hypothesis 2 was supported.

---

## Tables

### Table 1

*Means, Standard Deviations, and Correlations Among Study Variables*

| Variable | *M* | *SD* | 1 | 2 | 3 | 4 | 5 | 6 | 7 |
|----------|------|------|------|------|------|------|------|------|------|
| 1. Age | 24.36 | 6.90 | — | | | | | | |
| 2. Working hours | 33.73 | 21.92 | .26* | — | | | | | |
| 3. Organizational tenure | 6.13 | 9.96 | .54** | .24* | — | | | | |
| 4. Credit hours | 14.17 | 2.35 | -.19 | -.06 | .00 | — | | | |
| 5. Leader workaholism (cognitive) | 2.85 | 1.06 | .04 | -.04 | -.04 | -.05 | (.92) | | |
| 6. After-hours ICT use | 2.64 | 1.44 | -.04 | -.04 | -.05 | .20+ | .23* | — | |
| 7. Heavy menstrual bleeding | 2.49 | 1.03 | .01 | .05 | -.02 | -.19 | -.01 | .23* | — |

*Note.* *N* ranges from 69 to 86 due to pairwise deletion. Cronbach's alpha reported in parentheses along the diagonal.

\*\**p* < .01. \**p* < .05. +*p* < .10.

### Table 2

*Regression Results for Hypothesis Tests*

| | After-hours ICT use | | Heavy menstrual bleeding | |
|---|---|---|---|---|
| Predictor | *b* (*SE*) | *p* | *b* (*SE*) | *p* |
| Constant | 1.76 (0.47) | < .001 | 2.06 (0.30) | < .001 |
| Leader workaholism (cognitive) | 0.31 (0.16) | .048* | — | — |
| After-hours ICT use | — | — | 0.16 (0.08) | .048* |
| *R*² | .05 | | .05 | |
| *F* | 4.04* | | 4.05* | |

*Note.* *N* = 74.

\**p* < .05. +*p* < .10.

---

## Summary of Hypothesis Testing

| Hypothesis | Prediction | Result |
|------------|------------|--------|
| H1 | Leader workaholism (cognitive) → After-hours ICT use (+) | **Supported** (*b* = 0.31, *p* < .05) |
| H2 | After-hours ICT use → Heavy menstrual bleeding (+) | **Supported** (*b* = 0.16, *p* < .05) |

---

[Back to Project 4](project4.html)
