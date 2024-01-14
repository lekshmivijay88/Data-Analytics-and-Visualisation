# Data-Analytics-and-Visualisation
Data Analytics an Visualization on Stroke Data

##Aims and Objectives
The main objective of this project is to demonstrate my data analytics skills by applying appropriate data preparation techniques and performing detailed exploratory analysis on a healthcare dataset which in turn enables the visualization of valuable insights hidden in the data in the form of charts and plots. This project also aims to prove my ability to use multiple tools, techniques, and libraries used in the various stages of a data science project.

Accurate classification and identification of the people with a high risk of stroke can help to detect and treat the disease at an early stage thereby reducing the number of stroke deaths in the society.
This project involves the collection of the raw data related to stroke prediction, analyzing the prepared data to derive the information required to implement a stroke-prediction classification model based on ML algorithms. 

Data Source
The raw data for this study i.e., the stroke prediction dataset is downloaded from the Kaggle website as a CSV file. The “stroke” feature is identified as the target (dependent) variable and the remaining features are independent variables.

Data Preparation (Data Cleaning/Data Wrangling)
The first step is to analyze the data type and the statistics of each feature. 
![image](https://github.com/lekshmivijay88/Data-Analytics-and-Visualisation/assets/94902602/f138c436-96e4-40ae-9046-8d0747e5fab3)


Data Modelling
The entire dataset is split into training, validation, and test dataset in the ratio of 60:20:20. 
![image](https://github.com/lekshmivijay88/Data-Analytics-and-Visualisation/assets/94902602/ddbd0f52-8078-4544-af7e-c775581b69b2)

The optimal hyperparameter values for the RandomForestClassifier model are calculated using fivefold cross-validation implemented by the GridSearchCV class of the sklearn library. Finally, the best model is saved to a file with a pkl extension for future use.
 ![image](https://github.com/lekshmivijay88/Data-Analytics-and-Visualisation/assets/94902602/88168c8a-a3e8-44a4-a965-4a58081fc93f)

During the cross-validation process, the model is run for every possible combination of the specified parameter values and the most suitable one is determined.
![image](https://github.com/lekshmivijay88/Data-Analytics-and-Visualisation/assets/94902602/0436d40e-6e49-490b-9a47-8c704744397a)

Model Evaluation
The model was able to predict stroke with 96.7% accuracy on the validation dataset and 96.8% accuracy on the test dataset respectively. The precision and recall values are approximately the same on both datasets. But the metric specific for imbalanced datasets i.e., Index Balanced Accuracy (IBA) is 0.241 in the validation dataset and 0.938 in the test dataset.
![image](https://github.com/lekshmivijay88/Data-Analytics-and-Visualisation/assets/94902602/76dd52e6-c52d-4150-8710-5b6ce0bdc38c)

![image](https://github.com/lekshmivijay88/Data-Analytics-and-Visualisation/assets/94902602/0db954a8-47ba-40ab-8675-4f2ca66d54c9)

