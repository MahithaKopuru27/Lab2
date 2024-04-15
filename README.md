
## Random Forest Classifier for Assessment Scores

### Overview
This R script utilizes the `tidymodels` and `randomForest` libraries to train a random forest classifier on a dataset of assessment scores. The trained model is then used to make predictions on a separate testing set and evaluate its performance.

### Libraries Used
- `tidymodels`: For data splitting and model evaluation.
- `randomForest`: For building the random forest classifier.
- `ggplot2`: For data visualization.

### Data
The script assumes that the assessment scores dataset is stored in a CSV file located at `"C:/Users/mahit/OneDrive/Desktop/ml/oulad-assessments.csv"`. Ensure that the actual file path is updated accordingly.

### Workflow
1. **Data Preparation**: The dataset is read into R, and any rows with missing values are removed.
2. **Data Splitting**: The dataset is split into a training set (80%) and a testing set (20%) using stratified sampling based on the target variable `score`.
3. **Model Training**: A random forest classifier is trained on the training set using the `randomForest()` function.
4. **Prediction**: The trained model is used to make predictions on the testing set.
5. **Evaluation**: The predictions are compared against the actual values from the testing set to compute performance metrics such as accuracy, precision, recall, and F1-score using the `confusionMatrix()` function.
6. **Visualization**: The trained random forest model is visualized using a basic plot.

### Running the Script
1. Make sure to have R installed on your system.
2. Install the required libraries by running:
   ```R
   install.packages("tidymodels")
   install.packages("randomForest")
   install.packages("ggplot2")
   ```
3. Update the file path `"C:/Users/mahit/OneDrive/Desktop/ml/oulad-assessments.csv"` with the actual location of your dataset.
4. Execute the R script in your preferred R environment.

### Additional Notes
- Ensure that the target variable in your dataset is labeled as `score`.
