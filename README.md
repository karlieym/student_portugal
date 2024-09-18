# Exploratory data mining on secondary students in Portugal
## :pencil2: Project description
This project is for my education data mining course. Four data mining techniques are used to answer four research questions. The techniques are
**regression, random forest classification, relationship mining and PCA clustering.** Full code and paper can be found in this repository.
<br> The four research questions are:
<br> 1. Is it possible to predict student performance in Portuguese (mother tongue) Class? What are
the factors that affect student achievement?
<br> 2. Do the same analysis of students’ math final test performance, does it have the same attribution as Portuguese performance?
<br> 3. Can we find any interesting associations between other factors other than student’s academic performance?
<br> 4. What are the group characteristics of students with high and low grades respectively?

## :bar_chart: Data description
The data were obtained in a survey of students' math and Portuguese language courses in secondary school, which is available on [Kaggle.](https://www.kaggle.com/datasets/uciml/student-alcohol-consumption/data![image](https://github.com/user-attachments/assets/9c2f6b31-2166-44ea-8b09-a17536be2757)
) 
### Variables description

| Variable      | Description                                                                                      |
|---------------|--------------------------------------------------------------------------------------------------|
| `school`      | Student's school (binary: 'GP' - Gabriel Pereira or 'MS' - Mousinho da Silveira)              |
| `sex`         | Student's sex (binary: 'F' - female or 'M' - male)                                            |
| `age`         | Student's age (numeric: from 15 to 22)                                                         |
| `address`     | Student's home address type (binary: 'U' - urban or 'R' - rural)                             |
| `famsize`     | Family size (binary: 'LE3' - less or equal to 3 or 'GT3' - greater than 3)                   |
| `Pstatus`     | Parent's cohabitation status (binary: 'T' - living together or 'A' - apart)                   |
| `Medu`       | Mother's education (numeric: 0 - none, 1 - primary education (4th grade), 2 - 5th to 9th grade, 3 - secondary education, or 4 - higher education) |
| `Fedu`       | Father's education (numeric: 0 - none, 1 - primary education (4th grade), 2 - 5th to 9th grade, 3 - secondary education, or 4 - higher education) |
| `Mjob`        | Mother's job (nominal: 'teacher', 'health' care related, civil 'services', 'at_home' or 'other') |
| `Fjob`        | Father's job (nominal: 'teacher', 'health' care related, civil 'services', 'at_home' or 'other') |
| `reason`      | Reason to choose this school (nominal: close to 'home', school 'reputation', 'course' preference or 'other') |
| `guardian`    | Student's guardian (nominal: 'mother', 'father' or 'other')                                   |
| `traveltime`  | Home to school travel time (numeric: 1 - <15 min., 2 - 15 to 30 min., 3 - 30 min. to 1 hour, or 4 - >1 hour) |
| `studytime`   | Weekly study time (numeric: 1 - <2 hours, 2 - 2 to 5 hours, 3 - 5 to 10 hours, or 4 - >10 hours) |
| `failures`    | Number of past class failures (numeric: n if 1<=n<3, else 4)                                  |
| `schoolsup`   | Extra educational support (binary: yes or no)                                                  |
| `famsup`      | Family educational support (binary: yes or no)                                                |
| `paid`        | Extra paid classes within the course subject (Math or Portuguese) (binary: yes or no)         |
| `activities`  | Extra-curricular activities (binary: yes or no)                                               |
| `nursery`     | Attended nursery school (binary: yes or no)                                                   |
| `higher`      | Wants to take higher education (binary: yes or no)                                            |
| `internet`    | Internet access at home (binary: yes or no)                                                   |
| `romantic`    | With a romantic relationship (binary: yes or no)                                              |
| `famrel`      | Quality of family relationships (numeric: from 1 - very bad to 5 - excellent)                  |
| `freetime`    | Free time after school (numeric: from 1 - very low to 5 - very high)                         |
| `goout`       | Going out with friends (numeric: from 1 - very low to 5 - very high)                          |
| `Dalc`        | Workday alcohol consumption (numeric: from 1 - very low to 5 - very high)                     |
| `Walc`        | Weekend alcohol consumption (numeric: from 1 - very low to 5 - very high)                     |
| `health`      | Current health status (numeric: from 1 - very bad to 5 - very good)                          |
| `absences`    | Number of school absences (numeric: from 0 to 93)                                            |
| `G1`          | First period grade (numeric: from 0 to 20)                                                    |
| `G2`          | Second period grade (numeric: from 0 to 20)                                                   |
| `G3`          | Final grade (numeric: from 0 to 20, output target) |
                                              
## :bulb: Results and findings
### Findings regarding student final test grade(Q1&2):
1. Is it possible to predict student performance in Portuguese (mother tongue) Class? What are
the factors that affect student achievement?
<br> 2. Do the same analysis of students’ math final test performance, does it have the same attribution as Portuguese performance?
<br> Regression analysis was first carried out however the result is insignificant. Therefore, a random forest classification was carried out and luckily, the 
result was satisfactory. With 86% and 61.34% accuracy in predicting students' Portuguese and Math scores respectively.
<br> The following bar charts are the top ten contributing factors to our prediction:
<img width="632" alt="Screenshot 2024-09-17 at 19 14 25" src="https://github.com/user-attachments/assets/91dfe627-9f49-4eaa-a601-db1b14fecaa3">

<img width="632" alt="Screenshot 2024-09-17 at 19 17 18" src="https://github.com/user-attachments/assets/fc337531-d621-46ea-934e-05b93fbe4ff4">
<br>Students' performance in Portuguese is mainly influenced by family factors, such as family support, family size, parental relationship, etc. Students' math performance is also affected by school factors, such as the school they attend and school support. We can draw the rough conclusion that children from small, supportive, close-knit families have a better perception of language and words. Good math results are more dependent on the school, such as the quality of teaching, the degree of emphasis and other factors.
<br>

### Relationship mining findings(Q3):
3. Can we find any interesting associations between other factors other than student’s academic performance?
<br> The first and most obvious one is the **intention to pursue higher education**, since it has the most arrows pointing to it in the figure. Therefore, it can be concluded that students who **have access to the Internet** at home, who have attended **kindergarten**, and whose **families provide educational support** are most likely to want to pursue higher education. The second obvious conclusion is that Internet access is also favored by students who want to pursue higher education, who attended kindergarten and who had family educational support.
<img width="546" alt="Screenshot 2024-09-17 at 19 22 40" src="https://github.com/user-attachments/assets/a45edf81-0507-47fe-ada1-aad277d64ec7">

### PCA clustering findings
4. What are the group characteristics of students with high and low grades respectively?
<br> Students can be divided into 4 groups, below is a visualization of the clustering:
<img width="572" alt="Screenshot 2024-09-18 at 15 27 57" src="https://github.com/user-attachments/assets/ac3df88d-cd82-4434-922d-a1f59e077725">
<br> The top four features that contribute to clustering are **fathers being teachers, fathers working in health-related, Number of students in School Mousinho da Silveira and being guarded by moms.**
<br> <img width="556" alt="Screenshot 2024-09-18 at 15 32 22" src="https://github.com/user-attachments/assets/09fd2c53-a017-499b-8f5a-0ffcfa635d1d">
<img width="539" alt="Screenshot 2024-09-18 at 15 33 56" src="https://github.com/user-attachments/assets/be695790-6a29-43eb-91c7-eeca2040ab97">
<img width="529" alt="Screenshot 2024-09-18 at 15 34 36" src="https://github.com/user-attachments/assets/290a016d-dd7c-47f0-b369-5fe09c59583e">
<img width="553" alt="Screenshot 2024-09-18 at 15 35 37" src="https://github.com/user-attachments/assets/27ed143a-c60b-401d-8328-f7c85b636123">



