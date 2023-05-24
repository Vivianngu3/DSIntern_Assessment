# Data Science Intern Assessment


## Questions & Thoughts that I came across

- **What is Starcraft?**
 > Players are commanders leading one of three factions. The game revolves around gathering resources, building bases, training armies, and engaging in battles against other players or AI opponents. 
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
- Domain Knowledge: Think Starcraft

- **To what extent does the importance of variables change across levels of skill?**
- Not feasible to collect detailed data from across many levels of experience

- **Appropriate machine learning algorithm for Ordinal Regression?**
 > Classification- Categorise data based on predefined labels (Predicting and identifying categories such as ranks) 
 > ordinal logistic regression, support vector machines (SVM), or decision tree-based methods: ordinal random forest or gradient boosting

### Data finding Notes
- For the  Null values in some of the columns it would help to leave it blank instead of adding a question mark because when handling big data it would help the scientist faster detect and remove 
- Age, although it can be a good insight, might not be as practical or ethical to obtain since there is a population that would want to keep that information private.
- Null values all in LeagueIndex 8
- A large data gap collected in the lower LeagueIndexes (1-6) compared to the higher (7-8)
- LeagueIndex below 6 values are a lot smaller than 6 and above
- Compare "lower ranks"  1-5 with "higher ranks" 6-8

### Things to-do

- Watch and research Starcraft material, to get understanding of game
- Bookmark folder materials
- Set up Aneconda & jupyter notebook
- Refresh mind on Python setup
- Research Machine Learning models


### Data to-do
1. Data cleaning steps: Summary stats of each column, understand each column, finding & removing outliers, finding patterns

2. Transformations?

3. Feature selection: EDA Correlation plot for column selection, heatmap view. Maybe just 2 column plots- like a scatter plot between 2 columns. Selcted features 

4. What model to build?

5. Model performance

6. Next steps and take aways...
> Although I am not as proficient in Python functions, I have learned and adapted quickly to the situation and found resources necessary to help excel my work. I utilized my skills in UX Design and User research to curate and analyze holistic data. For the future I understand that reproducible code is important to be using it repeatedly. I want to further improve to be able to code more efficiently not for myself but for my team to have a easier time. 


