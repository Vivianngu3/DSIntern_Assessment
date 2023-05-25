# Data Science Intern Assessment


## Questions & Thoughts that I came across

- **What is Starcraft?**
    - Players are commanders leading one of three factions. The game revolves around gathering resources, building bases, training armies, and engaging in battles against other players or AI opponents. 
    - Resources around the map
    - Increase money and resources to build bases & units
    - A lot of macros to move around map faster 

- **What is PAC?**
> Perception Action Cycles (PACs). Actions and attention shifts for a typical StarCraft 2 player. "Most aspects of the PAC become faster with an increase in League."

- **How Can I determine the relevance of columns to the target variable (LeagueIndex)?**
    - Columns that have a weak or insignificant correlation may not provide valuable information for predicting the player's rank.
    - Redundant or highly correlated information. Removing redundant columns helps simplify the model and reduces the risk of overfitting. 
    - Remove Missing values or incomplete data. If a column has a significant amount of missing data, it might not be reliable or informative, and removing it can improve the model's accuracy.
    - Practicality and feasibility. If a column represents information that is difficult or costly to obtain, it may not be practical to include it in the model.
    - Domain Knowledge: Use research

- **To what extent does the importance of variables change across levels of skill?**
    Not feasible to collect detailed data from across many levels of experience

- **Appropriate machine learning algorithm for Ordinal Regression?**
    Classification- Categorise data based on predefined labels (Predicting and identifying categories such as ranks) 
    ordinal logistic regression, support vector machines (SVM), or decision tree-based methods: ordinal random forest or gradient boosting

### Data finding Notes
- Question Marks in place of nulls:
    - Ambiguity: Using a question mark as a placeholder for missing or null values introduces ambiguity in the dataset. It can be unclear whether the question mark represents a missing value, an unknown value, or a valid data entry. This ambiguity can affect the accuracy and reliability of any data analysis performed on the dataset.

    - Data Integrity: Mixing the question mark symbol with actual data values can hinder data integrity. It becomes difficult to distinguish between genuine data entries and the question mark placeholders. This can lead to incorrect data interpretations and analysis results.

    - Data Analysis and Operations: Many data analysis and statistical operations rely on the presence or absence of specific values. Using a question mark as a placeholder can interfere with these operations. For example, for calculations I came across unexpected results or errors when applied to data containing question marks.

    - Data Visualization: Plots, charts, and graphs often require consistent and valid data values to represent the underlying patterns accurately. Including question marks in the dataset may result in misleading or distorted visualizations.

    - Compatibility: Some data analysis tools, libraries, and algorithms may not handle question marks as null values by default. They may treat question marks as valid data points, leading to potential issues in data processing, modeling, or machine learning tasks.

- Age, although it can be a good insight, might not be as practical or ethical to obtain since there is a population that would want to keep that information private.
- Null values all in LeagueIndex 8, would need to eliminate those columns 
- There is a data LeagueIndex class imbalance. Indexes 1-6 have far higher rows than 7-8. Also, when trying to remove outliers, it removes all rows with index 6 & below showing a large difference for scale.
- Instead of removing outliers, work with normalizaiton to help with the difference in scale

### Things to-do

- Watch and research Starcraft material, to get understanding of game
- Bookmark folder materials
- Set up Aneconda & jupyter notebook
- Refresh mind on Python setup
- Make goals for data findings
- Research Machine Learning models


### Data to-do
1. Data cleaning steps: Summary stats of each column, understand each column, finding & removing outliers, finding patterns

2. Transformations?

3. Feature selection: EDA Correlation plot for column selection, heatmap view. Maybe just 2 column plots- like a scatter plot between 2 columns. Selcted features 

4. What model to build?

5. Model performance

6. Next steps and take aways...
    Although I am not as proficient in Python functions, I have learned and adapted quickly to the situation and found resources necessary to help excel my work. I utilized my skills in UX Design and User research to curate and analyze holistic data. For the future I understand that reproducible code is important to be using it repeatedly. I want to further improve to be able to code more efficiently not for myself but for my team to have a easier time. 


