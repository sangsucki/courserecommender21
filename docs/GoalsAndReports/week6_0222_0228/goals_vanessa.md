# Goal 1: Finalize Tableau Dashboards

After showing Frank the two Tableau dashboards for major selection and course planning (`02_eda/EDA_2013_2020.twb`), he really liked it and thought that it could be a useful final product. We are meeting next week with someone who could help us load our Tableau dashboard onto Duke's site so that it could be eventually be usable for students/advisors. To prepare for that, I need to clean up the dashboards and make them more user-friendly. This includes unlinking the two dashboards so that courses entered in one dashboard don't change the next dashboard. Also, I want to make them more visually appealing: change colors, reorient boxes, and ensure fonts/labels are clear/appropriate. Overall, this works towards the main project goal of __tracking academic pathway__. Furthermore, these dashboards help students select a major, choose classes to take next based on classes they've already taken, as well as plan when (what semester) to take those classes. I aim to have this done by __Thursday__. 

[Ilona great! the goal has a tangible outcome! It is clearly related to the big picture. Way to go!]

# Goal 2: Wireframe for Website

Because we are meeting with someone who will help us make our Tableau dashboards accessible to others on the Duke website, we as a team want to create a wireframe of what we envision the implementation of the dashboards to look like. This is similar to what we have done in our previous Data Visualization class with Jana and Ryan last year. Essentially, this would mean creating a prototype website by either drawing, using Google slides, or even other prototyping tools (Adobe, Figma) to create an outline of what the dashboards would look like on a website and how a user would interact with it. We want this to be done by Sunday so that we can send it to Frank and his contact on Monday before our Tuesday meeting. 

Example: website wireframe[https://www.freecodecamp.org/news/designing-a-website-ui-with-prototyping/]

# Goal 3: Alluvial Plots

This week, I aim to make the alluvial plots more user-friendly and understandable. I also want to use DSS to enable easier filtering. See details below. Overall, the alluvial plots contribute to the main project goal of tracking academic pathway, as it helps visualize the progression from one class to another. 

## Sub-Goal 3.1: Interactive Alluvial Plots

Though I was successful in creating alluvial plots in R, these plots are not interactive. My goal this week is to create alluvial plots that are interactive: show class and number of students when hovering, highlight path from class to class. From reading blogs, I know that this can be done in plotly, so I will work on changing the alluvial plots to work interactively through plotly. This is helpful because it makes the plots easier for others to understand and doesn't use R, which makes the DSS streamlining process easier since we will not have to create a new R environment. I aim to have this done by __Friday__. 

Reference for Plotly interactive alluvial plots: https://medium.com/plotly/4-interactive-sankey-diagram-made-in-python-3057b9ee8616 

## Sub-Goal 3.2: Streamline on DSS

I want to add the code to format the data and create the plots onto Dataiku DSS. This would be helpful because it would enable easy major filtering. Currently, the plots are only on the econ subset, but can easily be used for all other majors. Instead of programming this manually, DSS can provide an easy filtering method for major selection. This is done through the following steps:

1. Upload the data containing all majors (Note: because DSS is on a local Duke server and is protected with Shibboleth, Frank has approved of this upload.)
2. Create a filter recipe: https://knowledge.dataiku.com/latest/courses/visual-recipes/flights/filter-recipe-summary.html?highlight=filter. This is helpful because it will enable application to all majors rather than just econ. 
3. Upload python notebook with data formatting code (`03_intermediate/alluvial/alluvial_data.ipynb`). 
- If Sub-Goal 3.1 of creating Interactive Alluvial Plots is successful, then this notebook will also include plotting code. 
- If not, current working alluvial plot code is in the R file (`03_intermediate/alluvial/network_viz.Rmd`). This can be uploaded to DSS next to create non-interactive alluvial plots. I would also need to create a new R environment and would need to ask Darien to do so because of permissions on DSS.

I aim to have this done by __Tuesday__. 

[Ilona: awesome! I really like the goals, everything is clear and related to the overall story] 
