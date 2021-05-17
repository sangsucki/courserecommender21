## We have two ultimate goals for this project: 1) Improve prediction accuracy, 2) find academic trajectories. 

### 1-i) Create a python library for our neighborhood method. 
Since we have a sufficient accuracy for our neighborhood method, I would like to begin creating a python library. Users would type parameters such as major, how many classes they want to be recommended, semester, etc. and they would be able to have their class recommendations. If this is done within the next 2 weeks, I hope to implement it in demo webpage and see people’s feedback. This will be the demo version of our first ultimate goal for the project
[Ilona: Great! Good to see that you found the final model for the recommendation system]

### 2-i) measure robustness of the network structure and clustering classes
Looking at alluvial plots is effective but it’s hard to compare with our eyes which major is more structured than other majors. For this reason, my next goal is to figure out the robustness and compare majors in terms of their performance and robustness. Once I obtain robustness, called ‘modularity’, my assumption is that a major with more robust trend(modularity) is more likely to perform better accuracy. I found a research paper ‘Flows and Boundaries: A Network Approach to Studying Occupational Mobility in the Labor Market’. I chose this because it used data with temporal aspects and different modularity. I believe this paper discusses how to measure modularity and how to cluster different occupational mobility, which can be applied to class mobility. Using these two methods, first, I hope to compare majors in terms of modularity and see if our recommendation is affected. Second, I hope to cluster by a certain criteria and apply those clusters in the alluvial plots to illustrate the trend clearly. This result will support our report in terms of network approach. This will be done for the next two weeks.

[Ilona: Great explanation, I enjoyed learning more about the next steps you are taking! here is a recommendation take it or leave it: consider simplify plots, for instance, have them only for main classes of the major, predict only some majors that have a more clear path, exclude people with double majors, etc.]
