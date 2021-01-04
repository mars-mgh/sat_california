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

Generally speaking, you will be asked to come up with a data science problem. This problem is ultimately up to you, but below are some guidelines/things to consider when crafting a problem statement:
> 1. Consider your audience. Who is your project going to help? Who will your presentation be geared towards? Establishing your audience first can help you narrow down your scope.
> 2. Consider the data you will use. Based on the contents of this data, think about some questions you could reasonably answer. These questions should aim to solve some kind of problem.
> 3. Based on these questions, what would bring some kind value to your audience? This can be business insights, increase sales, make decisions, etc.
> 4. Put everything from the above steps together into a few sentences that describe the specific problem you are trying to solve and who it will benefit.
> [Here is a blog post](https://towardsdatascience.com/defining-a-data-science-problem-4cbf15a2a461) about crafting a data science problem statement.

Here are some example prompts if you need inspiration:
> * The new format for the SAT was released in March 2016. As an employee of the College Board - the organization that administers the SAT - you are a part of a team that tracks statewide participation and recommends where money is best spent to improve SAT participation rates. Your presentation and report should be geared toward non-technical executives with the College Board and you will use the provided data and outside research to make recommendations about how the College Board might work to increase the participation rate in a *state of your choice*.
> * You work for a school district that has asked you to advise their high school students on what SAT or ACT score they should be aiming for based on their intended area of study or school preferences.
> * You are hired by the state of California to analyze standardized test performance for various districts in the state and identify trends so they can allocate resources appropriately.
> * Lately, more and more schools are opting to drop the SAT/ACT requirement for their Fall 2021 applications ([*read more about this here*](https://www.cnn.com/2020/04/14/us/coronavirus-colleges-sat-act-test-trnd/index.html)). You are hired by a college to advise their admissions team on why this should or should not continue beyond the Fall 2021 applications. (Note: problem statements related to this prompt may not be reasonable to answer just using the data provided. If you want to tackle this one, you may need to find additional data online.)
> * *Feel free to be creative with your own prompt!*

And here are some example problem statements related to the above prompts. Come up with your own or modify these for your needs, do not just copy the ones given here:
> * The new format for the SAT was released in March 2016. Since then, levels of participation in multiple states have changed with varying legislative decisions. This project aims to explore trends in SAT and ACT participation for the years 2017-2019 and seeks to identify states that have decreasing SAT participation rates.
> * High school students often know which colleges they would like to consider, but rarely know what SAT or ACT score they should aim for when applying to these colleges. We wish to explore the schools that have the highest and lowest SAT and ACT score requirements and see if there is a relationship between college prestige and test scores.
> * The state of California has many school districts. This project aims to identify the districts that have the worst overall student performance on the SAT and ACT tests so the state can recommend programs and allocate resources to these districts in need. 
> * We hypothesize that student performance on these tests is not an indicator of overall academic performance. This project seeks to see if a relationship exists between student GPA and SAT/ACT scores to support or oppose the continuation of these tests as a requirement for college applications.
> * *Feel free to be creative with your own problem statement!*

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

### Conclusions

##### 1. Free SAT is not increasing participation
SAT has been offered for free since 2016 by counties around the State and overall they don't seem to be long term, neither in terms of participation.

##### 2. Free SAT  does not seem to be improving performance
SAT has been offered for free since 2016 by counties around the State and overall they don't seem to be long term, neither in terms of performance.

##### 3. Suggested Action: Math 
SMUH have been performing above average in the State, but strengthening Math skills can significantly improve students success rate in SAT.