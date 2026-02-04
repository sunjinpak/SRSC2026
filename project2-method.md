---
layout: default
title: Project 2 - Method and Results
---

[Back to Project 2](project2.html)

# Method and Results - Project 2

**Title**: The impact of leader workaholism on working students' emotional exhaustion and school withdrawal

**Team**: Jesus & Eric

**Style**: APA 7th Edition (JAP format)

---

## Method

### Participants

Participants were 115 working students recruited from a public university in the western United States. Eligibility criteria required that participants be currently employed and enrolled in college courses at the time of the study. The sample was 80% female, with an average age of 24.91 years (*SD* = 6.98). Regarding race and ethnicity, 55.7% identified as Hispanic or Latino, 15.7% as White, 7.0% as Asian, 3.5% as Black or African American, and 18.1% as multiracial or other. Participants worked an average of 37.05 hours per week (*SD* = 22.68) and were enrolled in an average of 14.20 credit hours (*SD* = 2.57).

### Procedure

Data were collected via an online survey hosted on Qualtrics. Participants were recruited through the university's participant pool. After providing informed consent, participants completed measures assessing their perceptions of their supervisor's workaholism, their own after-hours technology use, emotional exhaustion, and school withdrawal behaviors. All procedures were approved by the university's Institutional Review Board.

### Measures

Unless otherwise noted, all items were rated on a 5-point Likert-type scale ranging from 1 (*strongly disagree*) to 5 (*strongly agree*).

**Leader workaholism (cognitive).** Participants rated their supervisor's cognitive workaholism using four items from the cognitive subscale of the Multidimensional Workaholism Scale (Clark et al., 2020). This subscale captures the extent to which supervisors appear to think compulsively about work. A sample item is "It feels like my supervisor cannot stop themself from thinking about working" (α = .93).

**After-hours information and communication technology (ICT) use.** After-hours ICT use was assessed with a single item asking participants how often they used work-related ICTs (e.g., email, messaging apps, phone calls) outside of formal work hours in the past week (Boswell & Olson-Buchanan, 2007). Response options ranged from 1 (*never*) to 5 (*almost always*).

**Emotional exhaustion.** Emotional exhaustion was measured using five items adapted from the Maslach Burnout Inventory (Maslach & Jackson, 1981). A sample item is "I feel emotionally drained from my work" (α = .94).

**School psychological withdrawal.** School psychological withdrawal was assessed using eight items adapted from Hanisch and Hulin's (1990, 1991) withdrawal behavior measures, modified to reference school rather than work contexts. A sample item is "I have thoughts of being absent for the class." Response options ranged from 1 (*never*) to 5 (*always*; α = .83).

**Control variables.** We included several control variables that may influence the study variables. Age was included because older students may have developed more effective coping strategies for managing work-school demands (Butler, 2007). Gender was controlled for because prior research has found gender differences in emotional exhaustion (Purvanova & Muros, 2010). Weekly working hours was included because longer work hours are associated with greater strain and reduced capacity for nonwork activities (Sparks et al., 1997). Finally, credit hours enrolled was controlled for because heavier course loads may independently contribute to school withdrawal behaviors.

### Analytic Strategy

Analyses were conducted using Python 3.13 with the pandas, NumPy, SciPy, and statsmodels libraries. First, we computed descriptive statistics and bivariate correlations among all study variables. Second, we assessed the reliability of multi-item scales using Cronbach's alpha. Third, we tested our hypotheses (Hypotheses 1–3) using hierarchical ordinary least squares regression, entering control variables (age, gender, working hours, credit hours) in Step 1 and the focal predictor in Step 2. Given the exploratory nature of this study and the relatively small sample size, we evaluated statistical significance at the *p* < .10 level (cf. Aguinis et al., 2010).

---

## Results

### Preliminary Analyses

Means, standard deviations, reliabilities, and intercorrelations among study variables are presented in Table 1. All multi-item scales demonstrated acceptable internal consistency reliability (α > .70; Nunnally, 1978). Consistent with our theoretical expectations, leader workaholism (cognitive) was positively correlated with after-hours ICT use (*r* = .25, *p* = .011) and emotional exhaustion (*r* = .26, *p* = .008). After-hours ICT use was positively correlated with emotional exhaustion (*r* = .39, *p* < .001). Emotional exhaustion was positively correlated with school psychological withdrawal (*r* = .24, *p* = .014). Notably, leader workaholism (cognitive) was not significantly correlated with school psychological withdrawal (*r* = .04, *p* = .651).

### Hypothesis Tests

Results of the hierarchical regression analyses testing Hypotheses 1–3 are presented in Table 2. Hypothesis 1 predicted that leader workaholism (cognitive) would be positively related to employees' after-hours ICT use. After controlling for age, gender, working hours, and credit hours, leader workaholism (cognitive) was positively related to after-hours ICT use (*B* = 0.36, *SE* = 0.12, *t* = 2.93, *p* = .004, 95% CI [0.12, 0.60]). The addition of leader workaholism to the model explained an additional 7.4% of variance in after-hours ICT use (Δ*R*² = .074, *F* change = 8.59, *p* = .004). Hypothesis 1 was supported.

Hypothesis 2 predicted that after-hours ICT use would be positively related to emotional exhaustion. Controlling for covariates, after-hours ICT use was positively related to emotional exhaustion (*B* = 0.35, *SE* = 0.08, *t* = 4.44, *p* < .001, 95% CI [0.20, 0.51]). The addition of ICT use explained an additional 15.4% of variance in emotional exhaustion (Δ*R*² = .154, *F* change = 19.76, *p* < .001). Hypothesis 2 was supported.

Hypothesis 3 predicted that emotional exhaustion would be positively related to school psychological withdrawal. After controlling for covariates, emotional exhaustion was positively related to school psychological withdrawal (*B* = 0.12, *SE* = 0.05, *t* = 2.34, *p* = .021, 95% CI [0.02, 0.22]). The addition of emotional exhaustion explained an additional 4.7% of variance in school psychological withdrawal (Δ*R*² = .047, *F* change = 5.50, *p* = .021). Hypothesis 3 was supported.

---

## Tables

### Table 1

*Means, Standard Deviations, and Correlations Among Study Variables*

| Variable                           | *M*   | *SD*  | 1     | 2     | 3    | 4    | 5     | 6     | 7     | 8     |
| ---------------------------------- | ----- | ----- | ----- | ----- | ---- | ---- | ----- | ----- | ----- | ----- |
| 1. Age                             | 24.91 | 6.98  | —     |       |      |      |       |       |       |       |
| 2. Gender                          | 0.80  | 0.40  | −.06  | —     |      |      |       |       |       |       |
| 3. Working hours                   | 37.05 | 22.68 | .35** | −.03  | —    |      |       |       |       |       |
| 4. Credit hours                    | 14.20 | 2.57  | −.09  | .12   | −.07 | —    |       |       |       |       |
| 5. Leader workaholism (cognitive)  | 2.91  | 1.08  | .05   | −.09  | .00  | −.09 | (.93) |       |       |       |
| 6. After-hours ICT use             | 2.69  | 1.41  | .10   | .14   | .03  | .20* | .25*  | —     |       |       |
| 7. Emotional exhaustion            | 3.19  | 1.22  | −.07  | −.16  | .03  | .19† | .26** | .39** | (.94) |       |
| 8. School psychological withdrawal | 2.24  | 0.66  | −.19† | −.23* | −.02 | −.13 | .04   | .05   | .24*  | (.83) |

*Note.* *N* = 105 (listwise). Cronbach's alpha reliability coefficients appear in parentheses along the diagonal. Gender was coded 0 = *male*, 1 = *female*.

†*p* < .10. \**p* < .05. \*\**p* < .01.

---

### Table 2

*Hierarchical Regression Results*

| | After-hours ICT use | | Emotional exhaustion | | School psychological withdrawal | |
|---|---|---|---|---|---|---|
| Predictor | *B* (*SE*) | 95% CI | *B* (*SE*) | 95% CI | *B* (*SE*) | 95% CI |
| **Step 1** | | | | | | |
| Age | 0.01 (0.02) | | −0.02 (0.02) | | −0.02 (0.01)* | |
| Gender | 0.52 (0.36) | | −0.45 (0.29) | | −0.31 (0.15)* | |
| Working hours | 0.00 (0.01) | | 0.00 (0.01) | | 0.00 (0.00) | |
| Credit hours | 0.11 (0.05)* | | 0.08 (0.05)† | | −0.04 (0.02)† | |
| *R*² | .069 | | .076 | | .112 | |
| **Step 2** | | | | | | |
| Leader workaholism (cognitive) | 0.36 (0.12)** | [0.12, 0.60] | — | — | — | — |
| After-hours ICT use | — | — | 0.35 (0.08)*** | [0.20, 0.51] | — | — |
| Emotional exhaustion | — | — | — | — | 0.12 (0.05)* | [0.02, 0.22] |
| Δ*R*² | .074** | | .154*** | | .047* | |
| Total *R*² | .143 | | .230 | | .159 | |

*Note.* *N* = 105. Unstandardized regression coefficients are reported.

†*p* < .10. \**p* < .05. \*\**p* < .01. \*\*\**p* < .001.

---

## Summary of Hypothesis Testing

| Hypothesis | Prediction | Result |
|------------|------------|--------|
| H1 | Leader workaholism (cognitive) → After-hours ICT use (+) | **Supported** (*B* = 0.36, *p* = .004) |
| H2 | After-hours ICT use → Emotional exhaustion (+) | **Supported** (*B* = 0.35, *p* < .001) |
| H3 | Emotional exhaustion → School psychological withdrawal (+) | **Supported** (*B* = 0.12, *p* = .021) |

---

## References (for this section)

- Aguinis, H., et al. (2010). Best-practice recommendations for estimating interaction effects using moderated multiple regression. *Journal of Organizational Behavior, 31*, 776-786.
- Boswell, W. R., & Olson-Buchanan, J. B. (2007). The use of communication technologies after hours: The role of work attitudes and work-life conflict. *Journal of Management, 33*, 592-610.
- Butler, A. B. (2007). Job characteristics and college performance and attitudes: A model of work-school conflict and facilitation. *Journal of Applied Psychology, 92*, 500-510.
- Clark, M. A., Smith, R. W., & Haynes, N. J. (2020). The Multidimensional Workaholism Scale: Linking the conceptualization and measurement of workaholism. *Journal of Applied Psychology, 105*, 1281-1307.
- Hanisch, K. A., & Hulin, C. L. (1990). Job attitudes and organizational withdrawal: An examination of retirement and other voluntary withdrawal behaviors. *Journal of Vocational Behavior, 37*, 60-78.
- Hanisch, K. A., & Hulin, C. L. (1991). General attitudes and organizational withdrawal: An evaluation of a causal model. *Journal of Vocational Behavior, 39*, 110-128.
- Maslach, C., & Jackson, S. E. (1981). The measurement of experienced burnout. *Journal of Organizational Behavior, 2*, 99-113.
- Nunnally, J. C. (1978). *Psychometric theory* (2nd ed.). McGraw-Hill.
- Purvanova, R. K., & Muros, J. P. (2010). Gender differences in burnout: A meta-analysis. *Journal of Vocational Behavior, 77*, 168-185.
- Sparks, K., Cooper, C., Fried, Y., & Shirom, A. (1997). The effects of hours of work on health: A meta-analytic review. *Journal of Occupational and Organizational Psychology, 70*, 391-408.

---

[Back to Project 2](project2.html)
