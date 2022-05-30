# School District Analysis

### Analysis on school district performance using Jupyter Notebook,  Pandas Library and Numpy library.

## Project Overview

The School Board would like to understand the impact of changing all the grade 9 math and reading scores at Thomas High School to NaN - we will now review how this change impact various parts of the analysis relative to when it was ran including the Thomas High School grade 9 scores.The School Board would also like to understand various performance metrics of different school districts and schools. We will first work with Maria to provide the initial analysis based on data collected from many students and schools across the school district.

While the School Board is pleased with the initial insight that we have provided in our work with Maria, whereas it has been identified that there appears to be some anomalies in the data, in particular in the math and reading scores of the grade nine students at Thomas High School. In order to ensure these results do not skew the analysis, the Board has asked us to again work with Maria to remove the impact of these results by changing all the grade 9 Thomas High School math and reading scores to NaNs.



## Purpose 

The purpose of this analysis is to aggregate the students and schools datasets and analyze data on students standardized math and reading scores from various schools in the selected districts. To showcase trends in school performance, the analysis focuses on the following.

1.  The district summary, which includes the total number of students, the total number of schools, total budget, math and reading averages, and math, reading, and overall passing percentages.
2. The school summary, which includes, school type, number of students, school budget, average math and reading scores and math, reading, and overall passing percentages for each school.
3.  The top 5 and bottom 5 performing schools, based on the overall passing rate.
4.  The  average math and reading scores for each grade level (9th, 10th, 11th and 12th) from each school.
5.  The math and reading scores grouped by the following.
    -   Spending ranges per students
    -   School size
    -   School type

The analysis will assist the school board and superintendent in making decisions regarding the school budgets and priorities.

## Background

The data is gathered in two different CSV files (school data and student data). This is raw data that has to be transformed in order to perform analysis and convey information. Those steps are performed in the so-called  *data-wrangling*  or  *data-munging* process and include the following.

-   Load and read raw data from csv files.
-   Inspect data 
-   Clean data 
-   Merge datasets
-   Perform calculations and create tables
-   Change layout and structure of data
-   Sorting and grouping data

## Resources 
-   Data Source: [schools_complete.csv](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/schools_complete.csv)
-   Data Source: [students_complete.csv](https://github.com/awalindeep/School_District_Analysis./commit/ddfe61648cdb98b46f5f77f2181b5645b808abb8)
-   Sofware: Jupyter Notebook
-   Library: Pandas
-   Library: Numpy
-   Language: Python 

## Results

There was an evidence of academic dishonesty for math and reading scores in  Thomas High School for ninth graders; therefore, the school board wants to uphold state-testing standards for this school only. The grades for math and reading in Thomas High School, 9th graders will be replaced with NaNs while keeping the rest of the data intact. In the analysis below is the comparison from both analyses before and after the replacement the grades with NaNs.

  **Replacing the missing values with NaNs.**

NaN stands for “not a number”. In performing calculations, unlike 0 (zero) NaNs are not considered in the sum, or the averages; therefore, missing values don't have an impact. Yet we need to be careful if we multiply or divide rows with NaNs, because the answer, in this case, will be NaN. It is important to know those properties in order to make the right decision about handling missing values and other anomalies in the data sets.



**1. The impact on district summary**

-   In this summary, almost no results were impacted by NaNs. Data from Thomas High School 9th grade had minimal impact on district Analysis.
-   Each metric decreased by less that 0.5 percentage point each (meaning scores changed by less than 0.5%
-  With only 461 students in grade 9 at Thomas High School, and given the total student count is 39,170, the grade 9 students only make up 1.2% of the total student count, so removing their math and reading scores can only impact the averages so much.

![DSSOG](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/Ditrict_School_summary_Original.png)

![DSSUD](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/Ditrict_School_summary_Updated.png)

Data Frame from analysis "The district summary" before and after replacement grades with NaNs.



**2. The impact on school summary**

-   In this summary, results for School summary remained unchanged.
-   Average math and reading scores remained unchanged.
-   Passing math and reading percentage remained unchanged as well.
-   Overall passing percentage had no impact either.

![SSOG](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/School_Summary_Original.png)

![SSUD](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/School_Summary_Updated.png)

Data Frame from analysis The School Summary for Thomas High School before and after replacement grades with NaNs.

**3. The impact on math and reading scores**

-   In this report, only grades from Thomas High school in 9th grade was affected for math and reading.
- Grade 9 students at Thomas High School have NaN's
-  Calculations in this analysis were performed separately for each class and each school; therefore, other graders and schools weren’t affected.

* Top 5

![MOG](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/Math_Score_Original.png)
![MUD](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/Match_Score_Updated.png)

* Bottom 5

![ROG](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/Reading_Score_Original.png)
![RUD](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/Reading_Score_Updated.png)

Data Frame from analysis "The average math and reading scores for each grade level from each school" before and after replacement grades with NaNs.

**4. The top 5 and bottom 5 performing schools, based on the overall passing rate**

-   The overall rating for Thomas High School changed slightly.
-   The school rank remained second after changing scores with NaNs.

![TOG](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/Top_School_Original.png)
![TUD](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/Top_School_Updated.png)
![BOG](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/Bottom_School_Original.png)
![BUD](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/Bottom_School_Updated.png)


**5. School performance impact based on school spending**

-   From the Data Frame we can see that Thomas High school falls into a category  _spending range per students $630-$644_.
-   Calculations are made separately for those categories; therefore, scores in this summary are affected only within a category with NaNs.
-   Each metric changing less than 0.1 percentage points or change of less than 0.1%.

![SOG](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/Spending_Summary_Original.png)
![SUD](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/Spending_Summary_Updated.png)

Data Frame from analysis "School performance based on school spend" before and after replacement grades with NaNs.

**6. School performance impact based on the school size**

-   From the Data Frame we can see that Thomas High school falls into a category  _medium size school (1000 - 2000 students)_.
-   Calculations are made separately for those categories; therefore, scores in this summary are affected only within a category with NaNs.
-   Each Metric was impacted by less than 0.1%. 

![SOG](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/School_Size_Original.png)
![SUD](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/School_Size_Updated.png)

Data Frame from analysis "School performance based on the school size" before and after replacement grades with NaNs.

**7. School performance impact based on the type of school**

-   From the Data Frame we can see that Thomas High school falls into a category  _Charter_  for school type.
-   Calculations are made separately for those categories; therefore, scores in this summary are affected only within a category with NaNs.
-   Again the overall impact to all metrics was less than 0.1%.

![SSOG](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/Scool_Type_Original.png)
![SSUD](https://github.com/awalindeep/School_District_Analysis./blob/AwalinGHMAIN/Resources/School_Type_Updated.png)

Data Frame from analysis "School performance based on the type of school" before and after replacement grades with NaNs.


## Summary

Since Thomas High School math and reading grades for 9th graders were replaced with NaNs, there are minor changes in the report.

* Due to no data availability for Thomas High school math and reading scores for 9th graders values had to be replaced with NaNs.
*  The overall impact on results due NaNs was very minimal. In each individual case it can be quantified as less than 1%. 
*  There were some changes in school summaries by spending per student, size, and type. Again, only categories that include Thomas High School were affected. Categories that were affected are:  _Spending Ranges (Per Student) $630-644_,  _Medium size schools (1000-2000) students_  and  _The Charter schools_.
