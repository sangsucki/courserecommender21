## We have two ultimate goals for this project: 1) Improve prediction accuracy, 2) find academic trajectories. 

## This week 1-i) Fine-tune the current neighborhood method and apply this model to the top5 major dataset 1-ii) Neural Collaborative Filtering  2-i) Dynamic network plot, 2-ii) Dynamic Network Plot

### 1-1) Fine-tune the current neighborhood method and apply this model to the top5 major dataset and CS and Mechanical Engineering.
For the goal 1)'improve prediction accuracy', we obtained the best accuracy as 47.6% at average per semester. When I confined courses as top 15 classes, instead of removing courses taken by fewer than N students, the neighborhood method 
performed 72.6% at average. I changed this parameter to make our condition consistent since different number of people has taken various classes depending on majors. For example, there are 20 classes taken by students who majored in Economics, whereas only 7 classes taken by students who majored in Education.
And I applied this model to top5 major dataset and obtained 52% accuracy at average per semester(saved in '~/03_intermediate/neighborhoood/top5/item-user_top5.ipynb'). This is because top5 majors may have disturbed our prediction rate. In the same manner, I applied this to CS and Mechanical Engineering and the model performed 70.4% at average((saved in '~/03_intermediate/neighborhoood/cs/item-user_cs.ipynb'). In conclusion, our neighborhood method is able to recommend well in single major, instead of multi majors. 

[Ilona: this is a decent achievement! Recommendations within a single major sound very useful. ]

### 1-2) Limitation of Neural Collaborative Filtering(NCF) 
I implemented a toy example of NCF algorithm using a music data example. However, as I run the model, I realized that the music sample data is not applicable to our current data since our data has temporal aspects such as different semesters and binary data whereas the music data has no temporal aspect and people’s preference score from 1 to 5. We could consider ‘grade’ as people’s preference score, but we learned from our previous SVD model that it seems not to guarantee good performance (less than 10% accuracy). I decided not to go forward this model.

[Ilona: interesting exploration!]

### 2-1) Dynamic Network plot
I contacted Niko Hobart, who is a founder of Duke Applied Machine Learning Group, and arranged our meeting about dynamic network plot. Unfortunately, since Niko Hobart’s work was done by Java script, we were not able to do the same method that he used. However, he was very excited about our work when we presented our findings and models. He showed his willingness to get his group’s feedback once we publish our demo for undergraduate students. 

[Ilona: awesome!]

Due to the technical issue for the dynamic network plot, I redirected my goal to our dynamic alluvial plot. Vanessa successfully has done to make dynamic alluvial plots and connected 8 different semesters in one plot. However, one of the challenging parts was that there are too many classes transitioned from previous classes, which makes a lot of mess in the plot. This led me an interesting question, which is also related to our final report. “How do we measure how ‘messy’ the structure of each major is?” In other words, “how do we measure the robustness for a trend?” For example, the transition trend for CS and ME from alluvial plot  look more robust than Econ with our eyes.If we are able to measure this, we can tell which major has a stronger structure than other majors and compare performance with this robustness, which can be related to our recommendation accuracy. This will be investigated in the next week.

