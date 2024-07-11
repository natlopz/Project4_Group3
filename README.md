# Project4_Group3
Module 23 - Final Project
The aim of our project is to uncover patterns related to patient no-shows in Colorado. We plan to utilize information such as age, chronic diseases, socio-economic factors, and geographical influences to help identify any relationships between such factors. 

https://www.kaggle.com/datasets/kanchana1990/colorado-healthcare-decoding-no-show-patterns?resource=download

We found a dataset on Kaggle that would assist us in answering these questions, but we had to clean the information first. The first thing we did to clean the data was remove rows that contain null values. Next we removed the decimal places in the “Age” column so that the output are whole numbers. Lastly, we rounded the “Distance to Facility” column to the first decimal place.

Data Model Implementation
	Before working through the data, first we executed data preprocessing. There were three phases to this step, the first being removing columns with high correlations. Next, we used cumulative distribution to find cutoff values to identify and replace infrequent categories. Lastly, we needed to ensure the target column (Appointment_Outcome) was correctly identified and processed. 
	Next we had to split the data and scale it. We split the data into feature arrays (X) and target arrays (Y). Then we further split the data into training and testing sets using “train_test_split”. Lastly we used Keras with multiple layers to define a deep neural network. Then we added batch normalization and dropout layers to prevent overfitting.

Data Model Optimization
	The first part of our data model optimization was to execute model compilation and training. First we needed to compile the model with the Adam optimizer and binary cross-entropy loss function.Then we implemented early stopping which was important to prevent overfitting. Lastly we had to train the model on the training data and validate it on the testing data.

Tableau Visualizations
	We used Tableau to create visualizations of our data to help show the results in a more digestible fashion. The first graph shows how employment status affects whether patients will show up for their appointment or not. The next graph shows the effect distance from the facility has on whether patients show up for their appointments. The last graph looks at chronic disease by age and gender.

 https://public.tableau.com/app/profile/natalie.lopez5565/viz/HealthcareData_17206573267830/IdentifyingNo-ShowPatterns?publish=yes
