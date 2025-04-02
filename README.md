"# Food-Classification-Model" 
1. First i have imported all the library.
2. loaded the database csv file.
3. checking the missing value percentage.
4. dropped columns where missing value>50%
5. dropped irrivelnt columns.
6. Fill numerical columns with mean & Fill categorical columns with mode
7. selecting categorical columns dynamically and applying one hot encoding on the categorical columns.
8. Checking feature correlation using heatmap.(Feature selection)
9. Since we dont have a healthy column we created one by checking energy cal < 250
10. creating a health score to define if a food is healthy
11. Splitting the data into training and testing sets.
12. Feature scaling normalization
13. Train model
