# New York City Schools, SAT Scores, and Demographics
A project exploring the relationship between SAT scores and demographics in NYC. In this project, I use pandas, numpy, and regular expressions to read in and clean survey data regarding the SAT. I attempt to find whether or not there is a correlation between demographic factors like race, age, income, and gender with SAT scores to determine if the SAT is a fair test. If certain racial groups perform better on the SAT, then we have some evidence that the test may be unfair. 

# Observations

![SAT Scores and Survey Takers Correlation](https://github.com/fvu958/NYC_Schools/blob/master/graphs/sat_score_survey_corr.png)
- There are high correlations between n_s, n_t, n_p, and sat_score. Since they are correlated with total_enrollment, the positive correlation makes sense.
    - It's surprising that the student response rate, or rr_s/the percentage of students that completed the survey is positively correlated with sat_score. This might indicate that students are more likely to fill out surveys if they believe they've done well or students who fill out surveys are more inclined to do well academically.
    - The saf_t_11, and saf_s_11, or how students and teachrs perceived safety also correlates with sat_score. Safe learning environments make it easier to teach and learn.
    - Interesting to note that how students perceive academic standards correlates with sat_score, but it's the opposite for how teachers and parents perceive academic standards (aca_t_11 and aca_p_11, respectively).

![SAT Scores and Safety Correlation](https://github.com/fvu958/NYC_Schools/blob/master/graphs/sat_score_safety_corr.png)
- There's a correlation between student saftey and sat scores, but it isn't that strong. There are a few schools with very high safety and sat scores and low safety and sat scores. No schools with an average safety score of 6.5 had a SAT score higher than approx. 1500.

![SAT Scores and Race Correlation](https://github.com/fvu958/NYC_Schools/blob/master/graphs/sat_score_race_corr.png)
- White and Asian students correlate positively with SAT scores. Conversely, black and Hispanic students at schools correlates negatively with SAT scores. This may be due to socioeconomic factors, poverty, less support, and more

![SAT Scores and Hispanic Enrollment Correlation](https://github.com/fvu958/NYC_Schools/blob/master/graphs/sat_score_hispanic_corr.png)
- A lower Hispanic student body correlates positively with higher SAT scores. There's also a cluster of schools that have a majority Hispanic student body with very low scores. We should explore further

![SAT Scores and Percentage of Female Students Correlation](https://github.com/fvu958/NYC_Schools/blob/master/graphs/sat_score_gender_corr.png)
- The plot above indicates having a higher percentage of female students in a school correlates positively with SAT scores. Opposite is true of males. The correlation for both, admittedly, is not very strong.

![SAT Scores and Percentage of Female Students Correlation Scatter Plot](https://github.com/fvu958/NYC_Schools/blob/master/graphs/sat_score_female_corr.png)
- There doesn't seem to be any real correlation between sat scores and female_per based on the scatter plot. There does, however, appear to be a a cluster of schools with high schools and a higher female percentage (60-80%).

![SAT Scores, Enrollment, and AP Tests Correlation](https://github.com/fvu958/NYC_Schools/blob/master/graphs/sat_score_enrollment_corr.png)
- The plot indicates there isn't a strong correlation between the percentage of students in each school that took an AP exam and total enrollment. Notable that there are a cluster of students in the 50% area that have very high SAT scores, and that there are schools where AP exam



Potential Next Steps:
- Determing wheter there's a correlation between class size and SAT scores
- Figuring out which neighborhoods have the best schools
- If we combine this information with a dataset containing property values, we could find the least expensive neighborhoods that have good schools.
- Investigating the differences between parent, teacher, and student responses to surveys.
- Assigning scores to schools based on sat_score and other attributes.
