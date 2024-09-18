# Exploratory data mining on secondary students in Portugal
## Project description
This project is for my education data mining course. Four data mining techniques are used to answer four research questions. The techniques are
**regression, random forest classification, relationship mining and PCA clustering.**
<br> The four research questions are:
<br> 1. Is it possible to predict student performance in Portuguese (mother tongue) Class? What are
the factors that affect student achievement?
<br> 2. Do the same analysis of students’ math final test performance, does it have the same attribution as Portuguese performance?
<br> 3. Can we find any interesting associations between other factors other than student’s academic per-formance?
<br> 4. What are the group characteristics of students with high and low grades respectively?

## Data description
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
                                              
