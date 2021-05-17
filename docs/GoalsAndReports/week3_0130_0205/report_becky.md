It has been established that two major goals for the project are (1) have a recommendation model that shows decent prediction accuracy in terms of course coverage, and (2) identify course paths or ptatterns taken by the students.

With respect to the overall objectives, the progress for the goals set at the beginning of the week are detailed below:

To be more relevant and up-to-date, the data from now on to use are changed to the current data. Some exploratory analysis on the course taking behaviors are done through the following:
- Clustering on students using students' attributes including one-hot-encoded major/minor and course information;
- Clustering on courses themselves with subject information;
- LDA topic modeling on the students with term frequencies of courses taken

It is found out that course clustering alone did not generate meaningful separations. One cluster of courses might still contain various subjects which may not lead to evident meanings. Clustering on students with one-hot-encoded information was hard to analysis as well. On the other hand, with pyLDAvis tool, I can visualize the topics identified through LDA with courses qualitatively. For economics major, for example, at year2 (which I assumed people would be more concentrated and less noise), people focuses on going to areas like math, entrepreneurship, intermediate-level economics, finance, and interest (where I did 5 topics). Although it should be noted that these are all eye-balled observations and not really quantitative to be proven to be true, it provides some sort of course taking directions that might exist in one particular year or overal. It might worth looking into what specific curriculum for particular majors to get a better understanding. The commit include a `clustering_econ.ipynb` under `/02_eda/` folder.

With regard to the modeling, the previously identified decision tree/logistic regression did not seem feasible after consulting with Darien from Dataiku (in `wide_deep_test_econ.ipynb` under `03_intermediate`). I am trying some deep learning related models such as wide and deep model. In the wide and deep model, a linear model with a wide set of co-occurrence features can memorize the feature interactions, while deep neural networks can generalize the feature patterns through low-dimensional dense embeddings learned for the sparse features. However, the initial accuracy without particular training seems pretty low. It could be the reasons that a different train/test split method was used and also the column(attribute) information was not correctly fed.

[Ilona: Great job! I am glad that you are finding new paths to explore]
