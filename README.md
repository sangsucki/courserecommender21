# Duke Registrar Recommender System

## Introduction
Currently, universities rely on academic advisors and students’ individual research to guide major and course selection. However, with thousands of possibilities, it is extremely time-consuming and difficult to search through all the options. Using historical enrollment and graduation data, we propose several tools to facilitate major and course selection for undergraduate students at Duke University. 

## [Data](00_data)
From the Duke Registrar, we have two datasets: one with degree data and a second with enrollment information, each spanning 2013 to 2020. The degree dataset contains graduation degree information, including graduated students' de-identified IDs, graduation year, and major, minor, certificate, or secondary degree descriptions. The second dataset contains all course enrollment information, including de-identified IDs corresponding to those in the degrees dataset in addition to course descriptions, grades received, and academic year and term for every course each student took at Duke. 

## [Major and Course Planning Dashboards](04_deliverables)
To track academic pathways, we constructed a series of Tableau dashboards to aid in major and course selection as well as course planning. [The dashboards](https://public.tableau.com/profile/vanessa.tang#!/vizhome/MajorCoursePlanning/MajorCourse) consist of five main page:
- **Home**: provides brief instructions on how to use the dashboards as well as a link to the feedback form
- **Major Selection**: shows top 10 most popular majors after entering classes already taken
- **Course Selection**: shows top 10 most popular classes to take for the selected major and term, as well as the total number of students who graduated with that major
- **Course Planning**: shows top 10 most common majors and a class timeline after entering the classes students plan on taking in the future
- **Feedback Survey**

## [Academic Trajectory Visualizations](03_intermediate/alluvial)
Academic trajectories can be defined as the progression of classes a student takes throughout their undergraduate career. This can be helpful in identifying common patterns of courses to take for each major, while identifying majors that may have more structure than others. In this project, we have implemented two major visualizations to highlight academic pathways over time.
- Network Plots
- Alluvial Plots

## Models
- [Neighborhood Method](03_intermediate/neighborhoood)
    - The neighborhood-based method is commonly adopted among collaborative recommendation approaches due to their simplicity and efficiency.
- [LightFM](03_intermediate/lightfm)
    - LightFM is one of the hybrid matrix factorization model that is able to integrate three pieces of information: the information on the student, the information on the course, and the interaction information of which students took which courses.
- [Singular Value Decomposition (SVD)](03_intermediate/svd)
    - SVD is a matrix factorization technique aimed at capturing latent features and used to predict ratings based on a users past items and ratings (used grades as proxy). 

Though theoretically SVD and LightFM present some advantages over neighborhood methods, implementation and testing of these models revealed that the neighborhood model with cosine similarity performed much better than the other two models. Thus, we chose the neighborhood model as the final recommendation algorithm.


## [Related Documents](docs)
- [Final Paper](docs/final_paper/final_paper_updated.pdf)
- [Presentation slides](docs/presentations)
