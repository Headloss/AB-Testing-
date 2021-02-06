# AB-Testing-
Michael Wu


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

### Background
Udacity, a online learning platform(MOOCs), is trying to test a website change that adds a question page "How long do you plan to spend in this course?" before letting users checking out and registering a certified course, in order to filter out less commited students, to increase the retention rate after registering. If the answer is larger than 5 hours per week, students will be able to check out as usual; Otherwise, students will be suggested to only take this course in a "No Certificate" way with no payment and coaching provided.

### AB Testing Process
Users are diverted by cookies or user-ids if enrolled, into control groups and experiment groups.

First we choose a few invariant metrics(number of cookies, number of clicks) to conduct sanity checks, to ensure there is no significant difference in data of control and experment groups from the beginning. And our 2 metrics all passed sanity checks(Probability of data in control groups lies within 95% Confidnce Interval, with 0.5 null assumption).

Then we choose a few evaluation metrics(gross conversion, retention, net conversion), to evaluate if such website change is resulting statisitical significant changes and even practical significant changes. And the result is that changes bewteen control and experment groups: not practically significant in metrics of retention or net conversion; practical significance in gross conversion, but negative changes. Thus, it is recommended not to launch this new feature of "asking about potential study time" on Udacity before checking out.  


### Other Techinical Details
Note: we are using analytical variance here, since unit of diversion(cookies) is larger in scope than unit of analysis(clicks, enrolments)

Sign Tests:
We conduct a sign test on day-by-day paired data on evaluation metrics, finding that only gross conversion metric is statistical significant. It shows in a more detailed daily data scope, only in gross conversion sees statistical significant changes, between control and experiment groups.

Bonferonni Correction:
Bonferonni correction works for controling Type One error regarding if any metric out of mutiple metrics are significant, while our experiment requires ALL evaluation metrics to be significant. Thus, Bonferonni correction does not apply here.

Sample Size Needed:









