# CA04 – Ensemble Methods 
## Data Source and Contents 

The dataset is obtained from the Census Bureau and represents salaries of people along with seven demographic variables. The following is a description of our dataset: 

• **Number of target classes**: 2 ('>50K' and '<=50K') [ Labels: 1, 0 ]

• **Number of attributes (Columns)**: 7 

• **Number of instances (Rows)**: 48,842 

The data is provided in a .csv file at "https://github.com/ArinB/MSBA-CA-Data/blob/main/CA03/census_data.csv?raw=true”, a Github location. Use the GitHub link in 
your Python code to “read” the data into a Data-frame. 

        url = "https://github.com/ArinB/MSBA-CA-Data/blob/main/CA03/census_data.csv?raw=true”
        census = pd.read_csv(url, encoding = "ISO-8859-1") 

Other content includes: 

1. ensemble_methods_answers.docx -> Word Document with answers to given questions 

----------------------------------------------------------------------------------------- 
## Computer Assignment Road Map

**Part 1:** Data Quality Analysis and Exploratory Data Analysis

    1. DQA: Find missing values, if any, outliers, descriptive statistics and perform necessary data cleansing. 
    2. EDA: Ensure that data is binned correctly.  Then, create stacked bar charts for each variable based on the 'y' column.  
    3. Our variables are currently type=object, so we must make them type=category in order to encode them in the next step
    4. Check that column types converted correctly
    5. Use encoding to change values to an integer
    6. Split data into test and train datasets based on flag column
    7. Create our test and train variables

**Part 2:** Finding Optimal Value of a key Hyper-Parameter

    1. Find the optimal value of max depth
    2. Create empty dictionary 
    3. Create for loop to iterate through the various max depth options 
    4. Visualize and evaluate 

**Part 3 and 4:** Building a Random Forest Model and Building AdaBoost, Gradient Boost and XGB Models

    1. Use these steps to build models and find optimal number of estimators for (Random Forest, AdaBoost, GB and XGB):  
      a. Import package needed for model
      b. Use steps from Part 2 to model, visualize and evaluate

**Part 5:** Performance Evaluation Comparisons  

    1. Create dataframe that outputs the Accuracy and AUC values for each classifier
    2. Compare the performance between all classifiers 

-----------------------------------------------------------------------------------------
## Additional Comments 
Google Colab File has been linked to this repository.  However, should you make any adjustments, create a copy of your own to edit. 
