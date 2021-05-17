With respect to the goals set, this week I have achieved the following:

I have modified and standardized the pre-processing for both SVD and LightFM method. The standardized preprocessing include a re-normalization with respect to individual courses instead of individual student as done previously, and an exclusion of 100 least popular courses during the recommendation process to limit the search space.

For SVD, the prediction accuracy remains consistently around 10-20% for the test dataset. There were significant improvement when increasing the number of recommended items for LightFM model with almost double the prediction accuracy (changing from k=15 to k=30 can up the prediction accuracy up to 20-30%). It should be noted that recommending courses that might have a higher grade is isolated from recommending the courses that the students take. So far the prediction accuracy metric we have been using is focusing on prediction instead of other aspects of the recommending items.

Overall, neighborhood method appears to have the highest prediction accuracy and is able to achieve up to 60% accuracy for particular terms. It might be due to the intrinsic property of neighborhood method where it collects the most similar courses to the courses that the student has taken before and therefore has huge improvement when limiting the search space to make the course selection process much more focused.

This week we also had a class presentation which most of the efforts were put in, including seeking advice from Ilona, PPT making and result summaries in presentable format. 

[Ilona: report is great, Becky! next time please add references to gitLab]
