## We have two ultimate goals for this project: 1) Improve prediction accuracy, 2) find academic trajectories. 

## This week 1-i) I improved the model prediction accuracy for 2013-2020 dataset, 2-i) I built a dashboard using tableau, iii) Capstone presentation

### 1-i) I improved the model prediction accuracy (27.6% higher) for 2013-2020 dataset:
For improving prediction accuracy, I Improved the model prediction using neighboring method  by limiting search space. Specifically, I removed courses taken by fewer than N students and it turned out that N=100 performed the best and I applied this model to the 2013-2020 dataset (Econ Subset) and overall average accuracy per semester is 47.6 % (highest one is 60.8%), which is 26.8% bigger than previous accuracy. I also learned that the accuracy of Neighboring method is not sensitive to the number of K, which is a number of recommended classes. Unlike SVD, smaller K still performed better than other models including SVD. However, Neighboring Method can’t consider multiple features such as grade and it is inefficient to compute the similarity if it runs in real-time basis. The code is saved in two different files. The baseline model using neighboring method without limiting searching space is saved in ‘item-user_econ-no control.ipynb’. Next, the model using neighboring method with limiting searching space is saved in ‘item-user_econ.ipynb’.

### 2-i) I built a dashboard using tableau:
 For finding academic trajectories,  I built a Dashboard using Tableau. The dashboard shows what percentage of degree that students have graduated depending on classes. If you choose one of degrees shown, people also can see when people who chose the degree has taken the class. I was able to create the dashboard with a single class and gave my idea to Vanessa and she completed the dashboard with multiple classes.

### 3. Capstone presentation: 
For Capstone presentation, my team had 1-hour-long meeting and got feedback from Ilona, our project manager. With two successful results above, we presented our presentation for 5 minutes and had positive feedback from the audience. The presentation is found in 'docs/presentations/spring_class_presentation.pptx'

[Good job, Sangseok!]
