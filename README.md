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

---

### Goal of the Project:

The goal of this project is to perform an analysis that help further leverage the College Scorecard data to evaluate 
different metrics (such as retention rate) that can maximize the common student's success when choosing an institution 
for undergraduate study.  The hope is this work provides interesting insights and questions that can be further 
developed by students, families, academic advisors/counselors and policy makers for further drill-down for more specific
student-centered circumstances.

---

### Data

The [College Scorecard data set](https://catalog.data.gov/dataset/college-scorecard), collected and made available by 
the U.S. Department of Education, contains annual statisticson all accredited institutions in the country offering 
undergraduate degrees.  The data used for analysis in this project is from the most  recent 2015-2016 school year.

The objective of the College Scorecard data set from the U.S. Department of Education is stated to "make it easier for
students to search for a college that is a good fit for them... so they can make more informed decisions about which 
college to attend."

The College Scorecard data for the 2015-16 academic year includes 1,777 features and 7,593 observations.  For detailed 
breakdown on the data, please refer to the documentation below.

[Data Documentation](https://collegescorecard.ed.gov/data/documentation/)

#### Link to Raw Data Download for College Scorecard

[Raw CSV Data](https://catalog.data.gov/dataset/college-scorecard)


#### Links to Relevant API Documentation for College Scorecard

[Documentation](http://api.data.gov/ed/collegescorecard/)

[Endpoint](http://api.data.gov/ed/collegescorecard/v1/schools)

#### License

Data is released for use in the U.S. public domain by the United States government.  Copyright and related rights 
are waived through the [CC0 1.0 license](https://creativecommons.org/publicdomain/zero/1.0/).


#### Special Considerations and Limitations

- There is considerable sparsity in the data set, as assessed in the data importation and cleaning steps seen later in 
the
['Final_Project_Report.ipynb'](https://github.com/samirpdx/data-512-final-project/blob/master/Final_Project_Report.ipynb) 
notebook. As a result this renders many columns as unusable but the scope of the work did not involve any modeling. 
Regardless, the data set should be able  exploratory and research analysis, data for interesting insights.
- The data set spans out to the 1995-96 school year.  Again, due to bandwidth, we will only be exploring the 2015-16 
academic year.

---

### Directory Structure
```
data-512-final-project/
  |- sample data/
     |- CollegeScorecardDataDictionary.xlsx
     |- MERGED2015_16_PP.csv
  |- Final_Project_Plan.ipynb
  |- Final_Project_Report.ipynb
  |- LICENSE     
  |- README.md
```

---

### Reproducibility Steps

Please reference the Jupyter Notebook,
['Final_Project_Report.ipynb'](https://github.com/samirpdx/data-512-final-project/blob/master/Final_Project_Report.ipynb),
to see detailed step by step instructions of how the steps in the analysis were performed.

NOTE: The properly follow these steps, a user will need to be familiar with the Python programming language, install the
Jupyter Notebook environment and install the _pandas_, _numpy_, _matplotlib_ and _seaborn_ Python packages.

Steps are broken out as follows:

    Step 1: Import Data
    
    Step 2: Data Cleaning
    
    Step 3: Exploratory Data Analysis
    
    Step 4: Research Analysis & Findings
    
    Step 5: Discussion & Implications

    Step 6: Conclusions
     
