# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Standardized Test Analysis

### Overview

The SAT and ACT are standardized tests that many colleges and universities in the United States require for their admissions process. This score is used along with other materials such as grade point average (GPA) and essay responses to determine whether or not a potential student will be accepted to the university.

The SAT has two sections of the test: Evidence-Based Reading and Writing and Math ([*source*](https://www.princetonreview.com/college/sat-sections)). The ACT has 4 sections: English, Mathematics, Reading, and Science, with an additional optional writing section ([*source*](https://www.act.org/content/act/en/products-and-services/the-act/scores/understanding-your-scores.html)). They have different score ranges, which you can read more about on their websites:
* [SAT](https://collegereadiness.collegeboard.org/sat)
* [ACT](https://www.act.org/content/act/en.html)

Standardized tests have long been a controversial topic for students, administrators, and legislators. Since the 1940's, an increasing number of colleges have been using scores from sudents' performances on tests like the SAT and the ACT as a measure for college readiness and aptitude ([*source*](https://www.minotdailynews.com/news/local-news/2017/04/a-brief-history-of-the-sat-and-act/)). Supporters of these tests argue that these scores can be used as an objective measure to determine college admittance. Opponents of these tests claim that these tests are not accurate measures of students potential or ability and serve as an inequitable barrier to entry. Lately, more and more schools are opting to drop the SAT/ACT requirement for their Fall 2021 applications ([*read more about this here*](https://www.cnn.com/2020/04/14/us/coronavirus-colleges-sat-act-test-trnd/index.html)).

**Focus: California**

University of California has announced a new test for its Admission Process by 2025.
UC decision is part of a wider debate in California: for two times the California Assembly has voted a Bill that would have replaced the California State Assesment Requirement (CAASPP) with SAT in Grade 12, but both times the bill was vetoed by the Governor (frist Brown, more recently Newsom).
Arguments in favour of CAASPP is that it should be less biased towards students from underrepresented social groups. Also, SAT has recently introduced a "Hardship Score" to normalize the diffculties some students have duing their highschool years.

Since 2016-17 some Counties and Districts decided to offer SAT for free to their students [*source*](https://www.documentcloud.org/documents/3914482-California-Districts-Free-College-Entrance2016-17.html).

The project compares participation rate and performace in these Districts with others in California, and in particolare with San Mateo Unionified School District.

### Problem Statement

This project compares ACT dn SAT results in the school districts and counties of California over three Accademic Years (2016/17, 2017/18 and 2018/19). The analysis at County and District level addresses San Mateo Union High School Union in understanding the efficacy of its support to students.

---

### Datasets

#### Data

There are datasets included in the [`data`](./data/) folder for this project. 

* [`sat_2017.csv`](./data/sat_2017.csv): 2017 SAT Scores by State ([source](https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/))
* [`sat_2018.csv`](./data/sat_2018.csv): 2018 SAT Scores by State ([source](https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/))
* [`sat_2019.csv`](./data/sat_2019.csv): 2019 SAT Scores by State ([source](https://blog.prepscholar.com/average-sat-scores-by-state-most-recent))
* [`sat_2019_by_intended_college_major.csv`](./data/sat_2019_by_intended_college_major.csv): 2019 SAT Scores by Intended College Major ([source](https://reports.collegeboard.org/pdf/2019-total-group-sat-suite-assessments-annual-report.pdf))
* [`sat_2019_ca.csv`](./data/sat_2019_ca.csv): 2019 SAT Scores in California by School ([source](https://www.cde.ca.gov/ds/sp/ai/) | [data dictionary](https://www.cde.ca.gov/ds/sp/ai/reclayoutsat19.asp))


### Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|**cds**|*object*|SAT|County/District/School Code|
|**ccode**|*object*|SAT|County Code|
|**cdcode**|*object*|SAT|District Code|
|**scode**|*object*|SAT|School Code|
|**rtype**|*object*|SAT|Record type; used for filtering for County District and School|
|**sname**|*object*|SAT|School Name|
|**dname**|*object*|SAT/free_sat|District Name|
|**cname**|*object*|SAT|County Name|
|**income**|*object*|SAT|Per Capita Annual Income in 2018|
|**year**|*object*|SAT|Test Administration Academic Year|
|**enroll**|*int64*|SAT|Enrollment of Grade 12|
|**num_tst_takr**|*int64*|SAT|Number of Test Takers of Grade 12|
|**pct_tst_takr**|*int64*|SAT|Percentage of Test Takers of Grade 12|
|**avg_scr_eng**|*float64*|SAT|The number of students meeting the Evidence-Based Reading & Writing (ERW) |
|**pct_erw_benchmark**|*float64*|SAT|The percent of students who met or exceeded the benchmark for Evidence-Based Reading & Writing (ERW)|
|**num_math_benchmark**|*float64*|SAT|The number of students who met or exceeded the benchmark for SAT Math test|
|**pct_math_benchmark**|*float64*|SAT|The percent of students who met or exceeded the benchmark for SAT Math test|
|**tot_num_both_benchmark**|*float64*|SAT|The total number of students who met the benchmark of both Evidence-Based Reading & Writing (ERW) and Math|
|**pct_both_benchmark**|*float64*|SAT|The percent of students who met the benchmark of both Evidence-Based Reading & Writing (ERW) and Math|

### Findings

The general trend of students taking SAT in G12, is descending from the AY 2017-18, with a significant consistent drop in every county in 2018-19.

Data show a negative trend in SAT performances over the three years analyzed.
Also, students achieve higher scores in English Reading and Writing than in Math, but the negative trend described is equally affecting both sections of SAT.

As this project addresses San Mateo Union High on wether to adopt a *free for all* SAT test policy, the project presents a series of analysis showing SAT performances in Discricts who adopted the policy vs San Mateo.

* The participation in San Mateo Union High is between 40 to 60% in the three years examined. Districts offering SAT for free reach peaks of higher participation around year 2, but the increase does not appear to be consistent, dropping almost everywhere in the AY 2018-19.

* About 80% of of students at San Mateo Union High have successfully met the benchmark over the examined period; in the districts offering the SAT for free performances are overall lower, and don't appear to be increasing over time.

### Conclusions

##### 1. Free SAT is not increasing participation
SAT has been offered for free since 2016 by counties around the State and overall they don't seem to be long term, neither in terms of participation.

##### 2. Free SAT  does not seem to be improving performance
SAT has been offered for free since 2016 by counties around the State and overall they don't seem to be long term, neither in terms of performance.

##### 3. Suggested Action: Math 
SMUH have been performing above average in the State, but strengthening Math skills can significantly improve students success rate in SAT.

### Possible next steps

From the present analysis, there is no prove of a correlation between income and performance at SAT at county level in California. Futher analysis could be made to identify oter factors that might influence positively or negatively the performances of students from an environmental perspective.
It would be interesting to relate the income and the rate of students enrolled in G12, to verify that this result is actually significant.