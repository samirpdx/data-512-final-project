# Analysis of Undergraduate Retention Rates at 4-Year Universities

## A6 - Final Project 
##### DATA 512 - Human Centered Data Science


### Abstract:

College selection can often be an overwhelming and stressful process for high school graduates in the United States. 
Every year, tens of millions of prospective students must weigh several selection factors such as tuition cost,
proximity, program reputation, and future success indicators such as average salary upon graduation. The decision of
selecting the right institution could result in greater chances of personal and financial success in the future.
While popular annual college rankings, such as those published by the U.S. News and World Report, are thought as a
useful guide for some students and parents, to others they provide only a one-size fits all solution for students.

To better understand success for the average prospective college student, we leverage the College Scorecard data set 
provided by the U.S. Department of Education.  We evaluate research questions in respect to the success indicator of
student retention rate at 4-year undergraduate programs, seeing if they are affected by institution control (public or 
private, for-profit or non-profit), locale (city, suburb, townships, rural areas) and financial aid distribution tools
(loans and Pell Grants).

Overall, we see in the research that institutions offering 4-year undergraduate degrees show retention rates are highest
for students attending full-time, in either public or private non-profit institutions, and which located in more
urbanized areas. We see when assessing financial aid that the results showed a negative correlation between an
institution's overall retention rate and financial aid offerings (both loans and grants respectively).
However, due to the complexity of financial aid distributions, their varying individual impact on a student and the
effect on an institution that has a student base that is primarily financial dependent, there remains a lot more
analysis required to further understand the dynamics that financial aid tools play in retention rate.

### Goal of the Project:

The goal of this project is to perform an analysis that help further leverage the College Scorecard data to evaluate 
different metrics (such as retention rate) that can maximize the common student's success when choosing an institution 
for undergraduate study.  The hope is this work provides interesting insights and questions that can be further 
developed by students, families, academic advisors/counselors and policy makers for further drill-down for more specific
student-centered circumstances.


###Data

The College Scorecard data set, collected and made available by the U.S. Department of Education, contains annual statistics
on all accredited institutions in the country offering undergraduate degrees.  The data used for analysis in this project is from the most  recent 2015-2016 school year.

The objective of the College Scorecard data set from the U.S. Department of Education is stated to "make it easier for
students to search for a college that is a good fit for them... so they can make more informed decisions about which 
college to attend."

The College Scorecard data for the 2015-16 academic year includes 1,777 features and 7,593 observations.  For detailed 
breakdown on the data, please refer to the documentation below.

[Data Documentation](https://collegescorecard.ed.gov/data/documentation/)


#### Links to Relevant API Documentation for College Scorecard

[Documentation](http://api.data.gov/ed/collegescorecard/)

[Endpoint](http://api.data.gov/ed/collegescorecard/v1/schools)

This data is made available via CC0 1.0 license.

#### License

To obtain this data, I used the following link to download the data file:

[College Scorecard from the U.S. Department of Education](https://figshare.com/articles/Untitled_Item/5513449)


    Data is released for use in the U.S. public domain by the United States government.  Copyright and related rights 
    are waived through the CC0 1.0 license.


### Overview

###### Note:  The contents of the research process can be found in the "Final_Project_Report.ipynb" notebook.  Below is
a brief overview of the process used.

The data set for the 

Next, a literature review was done to help inform context of the domain of the study, specifically factors that affect student 
retetion.  This allowed for formation of research questions and hypotheses on what factors affect student retention rate.

Then visualizations were created using the "Seaborn" package in Python for both exploratory and research related analysis.

Lastly, a holistic assessment of this study both in terms of the conclusions from the data, the limitations and steps going
forward are detailed..


#### Special Considerations and Limitations

- The API call for ORES prediction scores is sped up with several rev_id input values as opposed to one at a time. 
  This can be done by creating one long string of rev_id values with a delimiter in between.
- There will be some rev_id values without any associated prediction scores.  To handle these and prevent errors 
when making calls to ORES, a suggestion is to insert a try/except statement.
- The entire call (done in 100 rev_id chunks) will take about roughly 3 minutes.  It is recommended to use the Python
"pickle" package in order to avoid having to re-run the call.


Directory Structure
---------------------
```
data-512-a1/

  |- final_data/
     |- final_merged.csv
  |- images/
     |- articles_per_pop_bot10.png
     |- articles_per_pop_top10.png
     |- hqa_country_bot10.png
     |- hqa_country_top10.png
  |- imported_data/
     |- page_data.csv
  |- LICENSE     
  |- README.md
  |- hcds-a2-bias-in-data.ipynb
```

### Reproducibility Steps

Please reference the Jupyter Notebook, 'Final_Project_Report.ipynb', to see step by step instructions of the steps used
to perform the analysis.

NOTE: The follow these steps, a user will need to be familiar with the Python programming language, as well as the
Pandas, NumPy, and Seaborn packages.

Steps are broken out as follows:

    Step 1: Downloading Data Sets 
    
    Step 2: Data Cleaning
    
    Step 3: Exploratory Data Analysis
    
    Step 4: Research Analysis & Findings

    Step 5: Conclusions
     
    
### Attributions

Jonathan Morgan (Professor, DATA 512, Human Centered Data Science, University of Washington) and
Oliver Keyes (TA, DATA 512, Human Centered Data Science)for example source code provided for API data requests.
    - Specific attributes found in 'hcds-a2-bias-in-data.ipynb'

Additional instructions provided by [HCDS Fall 2017 - Course Wiki](https://wiki.communitydata.cc/HCDS_(Fall_2017)/Assignments#Weekly_reading_reflections).  CC-BY-SA 3.0