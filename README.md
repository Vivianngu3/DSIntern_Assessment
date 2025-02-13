# Data Science Intern Assessment

# Identify
What am I trying to solve? What data to I need to collect? 

**Business Task:** You’re given a dataset of Starcraft player performance data in ranked games. We want
to develop a model to predict a player’s rank using the information provided in the
dataset. 



## Questions & Thoughts that I came across

- **What is Starcraft?**
Being someone who is not knowledgeable about the game, I needed to do some background research in order to have a better understanding of my stakeholder and terminology I would be handling.

    - Players are commanders leading one of three factions. The game revolves around gathering resources, building bases, training armies, and engaging in battles against other players or AI opponents. 
    - Resources around the map
    - Increase money and resources to build bases & units
    - A lot of macros to move around map faster 

- **What is PAC?**
    - Perception Action Cycles (PACs). Actions and attention shifts for a typical StarCraft 2 player. "Most aspects of the PAC become faster with an increase in League."

- **How Can I determine the relevance of columns to the target variable (LeagueIndex)?**
    - Columns that have a weak or insignificant correlation may not provide valuable information for predicting the player's rank.
    - Redundant or highly correlated information. Removing redundant columns helps simplify the model and reduces the risk of overfitting. 
    - Remove Missing values or incomplete data. If a column has a significant amount of missing data, it might not be reliable or informative, and removing it can improve the model's accuracy.
    - Practicality and feasibility. If a column represents information that is difficult or costly to obtain, it may not be practical to include it in the model.
    - Domain Knowledge: Use research

- **To what extent does the importance of variables change across levels of skill?**
    Not feasible to collect detailed data from across many levels of experience

- **Appropriate machine learning algorithm?**
    Classification- Categorise data based on predefined labels (Predicting and identifying categories such as ranks) 
    ordinal logistic regression, support vector machines (SVM), or decision tree-based methods


### Things to-do
- Research Starcraft material, to get understanding of features in Data set
- Bookmark folder materials for references
- Set up Aneconda & jupyter notebook files and GitHub REPO
- Refresh mind on EDA steps
- Make goals for data findings
- Research Machine Learning models

# COLLECTING
The data set I will be using is on Starcraft players


# CLEANING
Creating queries to review the data set and identify any areas to improve in order to prepare for analysis.


### Data finding Notes
- Question Marks in place of nulls:
    - Ambiguity: Using a question mark as a placeholder for missing or null values introduces ambiguity in the dataset. It can be unclear whether the question mark represents a missing value, an unknown value, or a valid data entry. This ambiguity can affect the accuracy and reliability of any data analysis performed on the dataset.

    - Data Integrity: Mixing the question mark symbol with actual data values can hinder data integrity. It becomes difficult to distinguish between genuine data entries and the question mark placeholders. This can lead to incorrect data interpretations and analysis results.

    - Data Analysis and Operations: Many data analysis and statistical operations rely on the presence or absence of specific values. Using a question mark as a placeholder can interfere with these operations. For example, for calculations I came across unexpected results or errors when applied to data containing question marks.

    - Data Visualization: Plots, charts, and graphs often require consistent and valid data values to represent the underlying patterns accurately. Including question marks in the dataset may result in misleading or distorted visualizations.

    - Compatibility: Some data analysis tools, libraries, and algorithms may not handle question marks as null values by default. They may treat question marks as valid data points, leading to potential issues in data processing, modeling, or machine learning tasks.
    - Recommend to use standardized approaches, such as representing missing values with NaN (Not a Number) or None 
    - Null values all in LeagueIndex 8, would make the class imbalance worse if we eliminate the rows

- Age, although it can be a good insight, might not be as practical or ethical to obtain since there is a population that would want to keep that information private.
- There is a data LeagueIndex class imbalance. Indexes 1-6 have far higher rows than 7-8. This can be also be due to the % of players in each rank
- There is a scale difference bewteen some of the columns. Work with normalizaiton to help with the difference in scale among the columns


### Data Issues & Problem-solving
1. Object columns have quesiton marks:
    - Replace or remove

2. Class Imbalance:
    - Adjust the model weight
    - Work with SMOTE 

3. Classification Report:
    - Precision and F-score are ill-defined and being set to 0.0 in labels with no predicted samples (LeagueIndex 7 & 8).
    - Go back and check data analysis/cleaning (fix any removals)

### Next steps and take aways...
Although I am not as knowledgable in Machine Learning methods, I know I have the work ethic and strong independent learning to get as far as I can in solving the problem. I utilized my skills in UX Design and User research to better analyze the data and find key information. Although I could not fully get to solve the accuracy of my model, I have some ideas to help improve it:

- Further examining the outliers. Testing the threshold and type of removal. (IQR, Zscore)
- Possible normalization method for the scale difference. Although it might be needed, could end up being one way towards a solution
- Log Transformation: As seen in beginning, there were positively skewed data for some of the features.
- Testing out RFE to determine feature selections. I am new to this one but found it could be a solution.
- Possible Training & Testing data handling. I only used the main df all the way down. I could split the Training and testing data earlier on to help better train the model.
- Further Tuning the model. There are multiple paramaters that could be utilized that I do not know of YET.

In conclusion, I want to further improve to be able to code more effectively not for myself but for my team. Through this internship I hope to further learn, grow and be curious about the work I do!


