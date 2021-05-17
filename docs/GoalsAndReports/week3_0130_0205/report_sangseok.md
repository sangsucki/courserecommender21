So far, we have set our goal with our client: 1) improve accuracy of our recommendation model, 2) find academic trajectories. We have focused a lot on the first goal last semester, I am focusing on the second goal this semester and the concept of network analysis is appropriate since it captures not only features of data but relationships. Since we deal with classes, which consists of sparse matrix (0 or 1) , network analysis is designed to keep track of binary data. 

My work is seen in [add mobility matrix and papers relatted to that](b82a954028bece9e94f0f36fa4b5571866a78976)

(i) I preprocessed data (Econ subset from 200in order to analyze the network matrix. Specifically, I divided students by class year and transformed the data into sparse matrix (0 and 1). 

ii) I successfully created the mobility matrix according to the papers: 1) “Curricular Flows: Trajectories, Turning Points, and Assignment Criteria in High School Math Careers (Daniel A. McFarland, 2006)" , 2) "Vacancy chains (Chase, 1991)". Three mobility matrix from the first year to the second year were created: 1) all courses 2) classes given threshold (relationship >0.2) 3) top popular 10 courses

iii) I applied the seaborn plot to visualize the mobility matrix for the three matrix above


[Ilona: great! You have clear deliverables and achievements of last week! Citing papers is a good idea. For outside readers you need to go one step further and explain what (metrics) tell you that you were successful in creating the matrix]
