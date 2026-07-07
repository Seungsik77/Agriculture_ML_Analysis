**KMeansClusteringSwineData**
1. Loaded swine_marketing Dataset
- encoded categorical columns to numerical
- Imputed NaN values for missing data
- Scaled data in order to reduce outliers

2. Defined the KMeans Clustering method
- Started with k = 10 clusters

3. PCA Decomposition/Visualization
- Reduced the dataset to 2 Principal Components
- Calculated centroids
- Visualized the clusters

4. Listed out clusters for each variable
- Showed how each variable had clusters of similar values

5. Calculate Group Efficiencies
- Group Efficiency = TotalPigsProduced / TotalPigsIn
- Ranked clusters based on efficiency

**SwineDataAnalysis**
1. Loaded swine_marketing Dataset
- Returned dataset shape (3000 rows, 5 columns)

2. Visualized features based on classes
- Visualized a 3D matrix of Feeder pig, Market hog, and Cull sow classes based on other features

3. Initialized Decision Tree Classifier
- Split dataset into Train/Test sets

4. PCA Implementation
- Used PCA to reduce to 2 Principal Components
- Visualized results on 2D graph

5. Data Analysis
- Plotted Live Weight vs Value in USD
- Visualized distribution of Values in USD


**SireLineSignificance**
1. Loaded 2025SireLineUpdate_SYNTHETIC dataset
   
3. One Hot encoded categorical variables
   
5. Split the dataset into train and testing sets
   
7. Scaled data to optimize for the Random Forest Regressor
   
9. Used the Random Forest Regressor to extract Mean Absolute Error, Root Mean Square Error, and R2 value
   - The R2 value of 0.95 means 95 percent of variance of the dependent variables in the model can be explained by the independent variables.
     
10. Conducted ANOVA Tests between SIRELINE and these variables (PERCENT MORTALITY, AVERAGE DAILY GAIN, FEED COST, and PERCENT TOPS)
   - Returned p values and f statistics
   - Returned best sireline based on these comparisons
   - Graphed each sireline vs respective variables with matplotlib
     
11. All Sirelines were statistically significant (p-values < 0.05), meaning at least one of their means were statistically different from the others

12. Exported a DataFrame with results to "SireLineSignificance.csv"
