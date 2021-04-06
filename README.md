# School_District_Analysis
# Overview
The school district is reviewing standardized testing scores for reading and math among high schools in their district.  These scores are to be compared with school funding and size.  After the analysis, the school board identified factors that appears to be evidence of academic dishonesty within one of the highschools.  Additional analysis has been requested to help determine possible variances to the orriginal analysis results by isolating questionable data.  

# Resources:
## Data Sources: 
	students_complete.csv
	schools_complete.csv
## Software:
	Python 3.7.6
	Jupyter 3.0.11
	Pandas
	Numpy

# Results
1.  How is the district summary affected?

Due to the sample size of all schools in the district all scores and percentages were marginally affected.  Math average scores dropped 0.1, reading average scores remained  unchanged.  Percent passing math, reading, and overall changed by 1.1% negatively.  

District Summary
![district_summary](https://user-images.githubusercontent.com/79231355/113645214-16da0580-964c-11eb-8632-9553d18f1089.png)

District Summary post removal
![district_summary_post_removal](https://user-images.githubusercontent.com/79231355/113645216-180b3280-964c-11eb-915f-dc5c714db73b.png)


2.  How is the school summary affected?  

Only Thomas High School was affected by removal of 9th grade scores.  The percent passing for reading, math, and overall moved significantly lower.  The drop is due to inclusiong of 9th grade students without grades in the calculation for percent passing.  This shows negative bias for the mean. 

Thomas high School Summary

![Thomas_High_School_summary](https://user-images.githubusercontent.com/79231355/113645750-168e3a00-964d-11eb-9fd5-129330f6259e.png)

Thomas High School Summary post removal

![Thomas_High_School_post_removal](https://user-images.githubusercontent.com/79231355/113645754-1857fd80-964d-11eb-884b-9bf5772208a2.png)


3.  How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Replacement of the ninth graders' scores results in a marginal change in average scores, and no change in relation to other schools.  Thomas High School's possition among the district is unchanged based on scores.  

Math Scores by grade

![math_scores_by_grade](https://user-images.githubusercontent.com/79231355/113646292-29edd500-964e-11eb-9da2-8af3afd8187f.png)

Math Scores by grade post removal

![math_scores_by_grade_post_removal](https://user-images.githubusercontent.com/79231355/113646316-36722d80-964e-11eb-8f85-c15a6d0e43e9.png)

Reading Scores by grade

![reading_scores_by_grade](https://user-images.githubusercontent.com/79231355/113646331-3d00a500-964e-11eb-983d-6cd8f25f62e8.png)

Reading Scores by grade post removal

![reading_scores_by_grade_post_removal](https://user-images.githubusercontent.com/79231355/113646343-4558e000-964e-11eb-93c2-d4c5974aea22.png)

4.  How does replacing the ninth-grade scores affect the following:

a. Math and reading scores by grade-   Only 9th grade was affected, and only for Thomas High School which no longer has values.  The values for 10th, 11th, and 12th grades remain unchanged. 
	
b. Scores by school spending-  The average score and passing percentages for math, reading, and overall were marginally affected, but did not change the position of the school compared to other schools and their spending. 

Scores by spending

![scores_by_spending](https://user-images.githubusercontent.com/79231355/113646518-97016a80-964e-11eb-86de-581bbc3389e7.png)

Scores by spending post removal

![scores_by_spending_post_removal](https://user-images.githubusercontent.com/79231355/113646607-c1ebbe80-964e-11eb-887b-811fd8908f42.png)

	
c. Scores by school size- The average score and passing percentages for math, reading, and overall were marginally affected, but did not change the position of the school compared to other schools. 
	
Scores by school size

![scores_by_school_size](https://user-images.githubusercontent.com/79231355/113646611-c4e6af00-964e-11eb-9a64-35ce2fd0f5fe.png)

Scores by school size post removal

![scores_by_school_size_post_removal](https://user-images.githubusercontent.com/79231355/113646631-cd3eea00-964e-11eb-8cd3-5747bcebe046.png)

d. Scores by school type- The average score and passing percentages for math, reading, and overall were marginally affected, but did not change the position of the school compared to other schools. 

Scores by school type

![scores_by_school_type](https://user-images.githubusercontent.com/79231355/113646659-de87f680-964e-11eb-856a-51a5bb08d6a5.png)

Scores by school type post removal

![scores_by_school_type_post_removal](https://user-images.githubusercontent.com/79231355/113646681-ec3d7c00-964e-11eb-9e93-43ba7efdd15b.png)


# Summary
The only major change was noted in the school summary where the 9th grade students remained in the calculation for overall passing scores.  This greatly impacted the calculation negatively, moving the value from 97% to 65%.  However, when the 9th grade students were removed from the calculation, the results returned near where they began, indicating academic dishonesty was not evident.  
1.  Average scores and passing percentages greatly reduced after removing 9th grade scores due to inaccurate math based on student population for Thomas High School
2.  The same error also resulted in drops in average scores and percent passing through the charter schools group, medium sized schools group, and spending range $630/644.  This is due to Thomas High School belonging to these groups. 
3.  When the 9th grade students were removed from those calculations, it showed a marginal change in average scores and percent passing.  The subsequent values for the charter schools group, medium sized schools group, and spending range $630/644 returned to the original values as the variance was too small to impact these larger data sizes.
4.  After evaluation, it does not appear that the scores from the 9th grade for Thomas High School have enough evidence of academic dishonesty.

