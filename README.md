## Project Workflow

The project was completed through the following steps:

1. **Data Loading**
   - The dataset was loaded and explored to understand its structure, features, and target variable.

2. **Data Preprocessing**
   - The input features were separated from the target variable (**Performance Index**).
   - The dataset was prepared for modeling by organizing the feature matrix `X` and target vector `y`.

3. **Train-Test Split**
   - The data was split into training and testing sets using `train_test_split()`.
   - `test_size=0.2` was used, meaning **80% of the data was used for training** and **20% for testing**.
   - `random_state=42` was used to make the results reproducible.
   - `shuffle=True` was applied to randomly shuffle the data before splitting.

4. **Model Training**
   - Three regression models were trained on the dataset:
     - **Linear Regression**
     - **K-Nearest Neighbors Regressor (KNN)**
     - **Decision Tree Regressor**

5. **Model Evaluation**
   - Each model was evaluated using both **training score** and **testing score**.
   - The purpose was to compare model performance and select the most reliable one.

---

## Model Results

The following results were obtained after training and testing the models:

- **Linear Regression**
  - Train Score: **0.9887**
  - Test Score: **0.9890**

- **KNN Regressor**
  - Train Score: **0.9889**
  - Test Score: **0.9838**

- **Decision Tree Regressor**
  - Train Score: **0.9993**
  - Test Score: **0.9763**

---

## Final Conclusion

After comparing the three regression models, **Linear Regression** achieved the best overall performance with the **highest test score of 0.9890**.

Although the **Decision Tree Regressor** achieved the highest training score, its lower testing score suggests slight **overfitting**.  
The **KNN Regressor** also performed well, but it was still slightly lower than Linear Regression.

Therefore, **Linear Regression was selected as the final model** for this project because it provided the **best balance between training and testing performance** and showed the strongest generalization ability.

