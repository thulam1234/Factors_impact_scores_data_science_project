# Factors_impact_scores_data_science_project
#### Data mining final project 
####  Members: Thu Lily Lam, Phuong Anh Nguyen 
#### Tool: R programming 

### Objective: 

To identify factors that impact students’s grades to implement strategies to help improve students success in school which contribute to increase school overall rating 

### Data summary:

Hours_studied: amount of time students spend to study 

Attendance: How often a student attend class

Parental involvement: level of which parents involved in their child academic life

Access to resources: How easy and accessible is it to academic resources 

Extracurricular activities: Whether or not students participate in extracurricular that can enhance their academic and involvement in school

Sleep hours: Average number of sleep. Sleep is crucial for brain development.

Previous score: previous exam score

Internet access: Ability to access internet 

Teacher quality : Quality of teachers 

Peer influence: influence of peers on academic performance 

Physical activity : Average number of physical activity per week

MotivationLevel: Student's level of motivation (Low, Medium, High).

Tutoring Sessions: Number of tutoring sessions attended per month.

Family Income: Family income level (Low, Medium, High).

School Type: Type of school attended (Public, Private).

Learning Disabilities: Presence of learning disabilities (Yes, No).

Parental_Education_Level:	Highest education level of parents (High School, College, Postgraduate).

Distance from Home: Distance from home to school (Near, Moderate, Far).

Gender: Gender of the student (Male, Female).

Exam_Score: Final exam score.

### Data source:https://www.kaggle.com/datasets/lainguyn123/student-performance-factors

### Exploratory Data Analysis 

<img width="412" height="293" alt="Screenshot 2026-05-24 at 2 20 19 PM" src="https://github.com/user-attachments/assets/2925d9a7-d63b-4c68-a8f7-f1064ac95e8e" />

This chart shows that students who attend class more often usually get higher exam scores. The dots go a bit upward, meaning attendance helps, but the relationship isn’t super strong, just a small positive trend.


<img width="524" height="378" alt="Screenshot 2026-05-24 at 2 20 42 PM" src="https://github.com/user-attachments/assets/eb57c225-e712-4bc0-ab32-77a34ed45181" />


Here the dots clearly go up. Students who study more hours tend to score better. It’s a stronger relationship than attendance. More study time usually means higher grades.

<img width="379" height="267" alt="Screenshot 2026-05-24 at 2 21 18 PM" src="https://github.com/user-attachments/assets/4ed8f54c-7dde-4141-bc7e-53c97aee9882" />

Most students fall around the middle exam scores. The shape shows that not too many students score super low or super high, most are in the average range.

<img width="395" height="279" alt="Screenshot 2026-05-24 at 2 21 39 PM" src="https://github.com/user-attachments/assets/99dd6314-5596-429d-8673-ce4b770419e1" />

A lot of students study around 15-25 hours. Only a few study very little 


<img width="378" height="267" alt="Screenshot 2026-05-24 at 2 22 06 PM" src="https://github.com/user-attachments/assets/5c20190b-d731-492f-8f09-f339e76d53a5" />

Sleep hours are pretty spread out. Some students sleep less, some sleep more, but many stay in the 6-9 hour range. It looks balanced.

<img width="365" height="270" alt="Screenshot 2026-05-24 at 2 22 40 PM" src="https://github.com/user-attachments/assets/a80f1a30-fa4d-4fce-91f2-8a0923372c09" />

Attendance is mostly high. Many students attend class often, and only a few have low attendance.



Data Summary:

<img width="655" height="255" alt="Screenshot 2026-05-24 at 2 23 10 PM" src="https://github.com/user-attachments/assets/603edfa5-002c-4083-93bb-b870df1e4225" />

This table shows all variables and their ranges. It tells us the dataset is big and includes numeric and categorical info. 

<img width="641" height="374" alt="Screenshot 2026-05-24 at 2 23 34 PM" src="https://github.com/user-attachments/assets/c7d04434-c2de-495f-84ed-c6b64964b369" />


<img width="666" height="334" alt="Screenshot 2026-05-24 at 2 23 48 PM" src="https://github.com/user-attachments/assets/5f20f88c-d330-4432-b393-2e8797d5732b" />


<img width="672" height="307" alt="Screenshot 2026-05-24 at 2 24 02 PM" src="https://github.com/user-attachments/assets/ba1735b4-7ef7-4615-b49e-40757193eda0" />

Training data shows students usually study 16-24 hours, sleep 6-8 hours, and attend class 70-90%.
Previous scores average around 75, and exam scores in training are mostly 65-70.
Most students have internet, medium motivation, medium family income, and medium/high teacher quality.
Only a small group has learning disabilities, and most live near the school.


<img width="570" height="185" alt="Screenshot 2026-05-24 at 2 24 29 PM" src="https://github.com/user-attachments/assets/043709da-8311-4276-8c3b-bd304931e656" />


Average exam score slightly declines compared to the last exam. The previous score was 75.07, and dropped to 67.23 in the final exam. This could be due to various reasons. Linear Regression:

<img width="631" height="238" alt="Screenshot 2026-05-24 at 2 24 50 PM" src="https://github.com/user-attachments/assets/5ea2c686-0ab8-4f91-80f5-0b2d911345ad" />

<img width="633" height="238" alt="Screenshot 2026-05-24 at 2 25 26 PM" src="https://github.com/user-attachments/assets/26a364d6-19bf-4cd4-8688-58eb3c3188c8" />

<img width="505" height="390" alt="Screenshot 2026-05-24 at 2 25 44 PM" src="https://github.com/user-attachments/assets/338604ef-a14f-4e97-8e24-142a8556f29d" />

Evaluating the original with various methods including r-squared, adjusted r-squared, AIC and BIC. 

### Linear Resgression model 

<img width="542" height="623" alt="Screenshot 2026-05-24 at 2 26 32 PM" src="https://github.com/user-attachments/assets/0f1657c3-bc33-41c1-8ae7-8af08510dddd" />



The linear regression original model shows many significant variables. The two non-significant variables are sleep hours and type of school.

<img width="561" height="152" alt="Screenshot 2026-05-24 at 2 26 55 PM" src="https://github.com/user-attachments/assets/bdfabb11-b35e-4ea4-84ac-6e51e8eba9b3" />

The regression model shows that hours studied, previous scores, motivation, teacher quality, and attendance are strong predictors of exam scores. The R-squared is around 0.72, meaning the model explains a good amount of the score variation.

<img width="631" height="693" alt="Screenshot 2026-05-24 at 2 27 20 PM" src="https://github.com/user-attachments/assets/68c444f2-e3ec-49c5-a877-1a4748acf28c" />


The model’s error is around 4.28, and the cross-validation error is about 4.16. Shows the model predicts exam scores pretty well and is consistent.

<img width="682" height="557" alt="Screenshot 2026-05-24 at 2 27 44 PM" src="https://github.com/user-attachments/assets/fa0aa528-9d8e-4bb8-b8b0-f51c3aeb9971" />

Fitting the model shows the majority of the points fit the line, but some of them do not fit along the line, which indicates that the dataset is not normally distributed. 

<img width="759" height="280" alt="Screenshot 2026-05-24 at 2 28 15 PM" src="https://github.com/user-attachments/assets/0dd89fdc-850a-4488-a9ac-0d6eab4b2096" />

### Regression Tree model 

Regression tree model shows attendance and hours study are the two top predictors to the outcome. 

<img width="673" height="126" alt="Screenshot 2026-05-24 at 2 28 40 PM" src="https://github.com/user-attachments/assets/9e82fd19-e99f-4012-a667-e5f6e7cf2fb6" />


The MSE of the tree is 6.6, which is higher compared to the linear regression model. 

<img width="710" height="204" alt="Screenshot 2026-05-24 at 2 29 01 PM" src="https://github.com/user-attachments/assets/07d0dc35-497d-4e78-87bf-f3f49cfb50d8" />

The training model MSE is a bit higher than the big tree model, which shows the lower error in the bigger tree model.

<img width="689" height="233" alt="Screenshot 2026-05-24 at 2 29 32 PM" src="https://github.com/user-attachments/assets/4fec1080-f85e-4c7b-8409-c1d161eaa92c" />


### Random Forest 

<img width="677" height="565" alt="Screenshot 2026-05-24 at 2 30 27 PM" src="https://github.com/user-attachments/assets/c95693c2-b615-47cf-b25a-9b59ee38a57a" />

This random forest model shows a really stable MSE after 6 iterations. Mean squared residuals is 5.14, which indicates a stable and low error for this dataset.

<img width="642" height="281" alt="Screenshot 2026-05-24 at 2 30 46 PM" src="https://github.com/user-attachments/assets/de5ded87-0de1-46b9-b372-f39d701f7aeb" />

Important variables are ranked variables based on how important they are to the final decision. Model shows hours-Studied, attendance and previous score are the strongest predictors. 

<img width="655" height="268" alt="Screenshot 2026-05-24 at 2 31 04 PM" src="https://github.com/user-attachments/assets/481f48e9-700c-4498-8086-bb61b24c90e6" />


Random forest model shows a reduction of error at approximately 100 and slightly drop until its reaches 500 trees with the lowest error.

Conclusion:
Throughout this study, Hour study and attendance are the two strongest predictors to the final exam outcome. The best model to predict the outcome is linear regression and random forest, then regression tree model. 




























