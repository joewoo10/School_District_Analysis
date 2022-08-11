# School_District_Analysis

## Overview:
The school board would like to understand several performance metrics of the various schools in the district. While the school board is pleased with the initial analysis we have provided, it’s been brought to our attention that there is evidence of academic dishonesty, mainly in the math and reading scores of the ninth-grade students at Thomas High School. Therefore, the Board has asked us to eliminate the impact of these results by changing all the Thomas High School ninth-grade math and reading scores to null values and repeat the school district analysis.

## Results:

### Effect on district summary

The change of adding null values to all ninth-grade Thomas High School math and reading scores did not have a sizeable impact on the district analysis, with each metric decreasing by less than 0.5 percent. It should be noted there are only 461 ninth-grade students at Thomas High School, and given the total district student count is 39,170, the Thomas High School ninth-grade students comprise 1.2% of the total student count. Thus, the removal of their math and reading scores had little impact.

##### *Original District Summary*
![image](https://user-images.githubusercontent.com/109227896/184065073-eb693280-b342-49bb-af68-814d2d55a785.png)

##### *Adjusted District Summary*
![image](https://user-images.githubusercontent.com/109227896/184065221-54d97f2f-f3bb-4699-95c4-9719913db8ee.png)


### Effect on school summary

In the initial analysis, Thomas High School had a 91% overall passing rate, this concerned the school board as it seemed artificially high. Removing the ninth-grade students from the data set had a enormous impact, reducing the overall passing rate from 91% to 65%.

##### *Thomas High School with Ninth Graders Included*
![image](https://user-images.githubusercontent.com/109227896/184065508-2f259f44-d022-44fb-817c-6490677a6fc3.png)

##### *Thomas High School with Ninth Graders Removed*
![image](https://user-images.githubusercontent.com/109227896/184065681-c0693f95-8656-428f-975a-477ea0f82d66.png)


### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

While the average math, reading and overall scores at Thomas High School were impacted with the update, however the changes were not enough to alter its relative ranking versus the other schools. The changes resulted in a less than a one percentage point change for each metric.

##### *Original List of Top Schools*
![image](https://user-images.githubusercontent.com/109227896/184065885-75a86a24-2deb-4752-86e1-7ab15077283c.png)

##### *Adjusted List of Top Schools*
![image](https://user-images.githubusercontent.com/109227896/184066012-f68d56cd-c586-4901-bda1-42f3cfd54427.png)


### How does replacing the ninth-grade scores affect the following:

#### Math and reading scores by grade
- The only real change here is to the ninth-grade students at Thomas High School who have had their math and reading scores changed to the null value *Nan* (not a number). If we ran a sum or mean of the DataFrame, we would see a difference between the original and adjusted.

##### *Original Math Scores By Grade*
![image](https://user-images.githubusercontent.com/109227896/184066531-9ea90634-d013-417d-af2c-82431fa11d0a.png)

##### *Adjusted Math Scores By Grade*
![image](https://user-images.githubusercontent.com/109227896/184066613-89c9acb4-cac4-40bd-8e15-ea723b6cd011.png)


#### Scores by school spending
- There was only a slight change in the school spending groups scores for the $630-644/student range as this is where Thomas High School resides. As expected, this was a very small change of well below 1%.

##### *School Spending - Original*
![image](https://user-images.githubusercontent.com/109227896/184066977-38cb83e1-c885-4934-ba17-c1fd0a05899e.png)

##### *School Spending - Adjusted*
![image](https://user-images.githubusercontent.com/109227896/184066999-4d32bc80-72e2-4943-a098-8f2620cd4a27.png)


#### Scores by school size
- The scores for the Medium (1000 - 2000) school size changed ever so slightly (less than 1 percentage point, just as we have seen with previous results). Once again, this is due Thomas High School falling in this range with 1,635 students in attendance. 

##### *School Size - Original*
![image](https://user-images.githubusercontent.com/109227896/184067111-13df91c1-7e9e-4b17-8fe1-a10d0f1801b2.png)

##### *School Size - Adjusted*
![image](https://user-images.githubusercontent.com/109227896/184067118-62bf955b-1d67-454b-ba86-c0570b223473.png)


#### Scores by school type
- Thomas High School is a Charter school, therefore we only see changes to the scores for the Charter type. And yet again, the change is well below 1%. 

##### *School Type - Original*
![image](https://user-images.githubusercontent.com/109227896/184067175-08fbe407-ceee-442d-8c41-afc31a04aae5.png)

##### *School Type - Adjusted*
![image](https://user-images.githubusercontent.com/109227896/184067232-a78a3481-e270-44b3-9b78-6c3d4d9e39d9.png)



### Summary
- The overall passing rate for Thomas High School changed significantly from 90.63% to 65.08%.
- Top School Ranking - no change to ranking, however Thomas High School scores did change, but by less than 1 percentage point (or changed by less than 1%) for each metric.
- Scores by School Size - changes to Medium (1000-2000) grouping for all scores by less than 0.1 percentage points (or change by less than 0.1%).
- Scores by School Type - changes to Charter type grouping for all scores by less than 0.1 percentage points (or change by less than 0.1%).
