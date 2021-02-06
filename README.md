# AB-Testing-


## DESCRIPTIONS:


-Completed an A/B Test on a potential Udacity website interface change: add a free trial screener, to filter out students with less commitment to finishing courses, in order to improve retention rate


-Applied A/B test knowledge: invariant/evaluation metrics, unit of diversion/analysis, analytical/empirical variance, statistical/practical significance


-Applied A/B test skills: sign tests, sanity checks, sample size needed for statistical power, Bonferroni correction


## files:

-"Final Project": Instructions & descriptions of final project

-"Final Project_pdf": Summary of project results

-"Excel Calculations":
1. [Calculation of standard deviations, sample sizes needed](https://drive.google.com/file/d/10obHb4HIKd9ZEH41NjdLCU8MQAu560up/view?usp=sharing_)

2. [Calculation of sanity checks, evaluation metric effects, and sign tests](https://drive.google.com/file/d/1yzMcKPUNg5XqdqMet2bwrwEM8yWKBb70/view?usp=sharing)

## Project Summary:

An experiment was conducted in which potential Udacity students were diverted by cookie into two groups, experiment and control. The experiment group was asked to input the amount of time they are willing to devote to study, after clicking a "start free trial button", whereas the control group was not. Three invariant metrics (Number of Cookies, Number of clicks on "start free trial", and Click-Through-Probability) were chosen for purposes of validation and sanity checking while Gross Conversion (enrollment/cookie) and Net Conversion (payments/cookie) served as evaluation metrics. The null hypothesis is that there is no difference in the evaluation metrics between the groups, futhermore, a practical signifcance threshold was set for each metric. The requirement for launching the experiment is that the null hypothesis must be rejected for ALL evaluation metrics and that the difference between branches must meet or exceed the practical signficance threshold. Because our acceptance criteria requires statiscally signifcant differences for ALL evaluation metrics, the use of the Bonferonni correction is not appropriate. The Bonferonni correction is a method for controlling for type I errors (false positives) when using multiple metrics in which relevance of ANY of the metrics matches the hypothesis. In this case the risk of type I errors increases as the number of metrics increases (signifcance by random chance). In our case in which ALL metrics must be relevant to launch, the risk of type II errors (false negatives) increases as the number of metrics increases, so it stands to reason that controlling for false positives is not consistent with our acceptance criteria.

Analysis revealed the expected equal distribution of cookies into the control and experimental groups, for the invariant metrics, at the 95% CI. A difference in gross conversion was found to be statistically signficant at the 95% CI, and the null hypothesis was rejected. Gross conversion also met the practical signficance threshold. Net Conversion was found to be neither statistically nor practically signficant at the 95% CI.
