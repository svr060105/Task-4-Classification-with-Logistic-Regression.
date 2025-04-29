# Logistic Regression Binary Classifier

This project demonstrates how to build a binary classifier using **Logistic Regression** on the **Breast Cancer Wisconsin dataset**. The goal is to predict whether a tumor is **malignant (M)** or **benign (B)**.

---

## Dataset

I have used the [Breast Cancer Wisconsin (Diagnostic) Dataset](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)).
---

## Tools and Libraries

- **Python**
- **Pandas** – data handling
- **NumPy** – numerical operations
- **Matplotlib** – data visualization
- **Scikit-learn** – model building and evaluation

---

## Steps Followed

1. **Load and preprocess the dataset**
   - Drop irrelevant columns like `id`
   - Map diagnosis labels: `'M'` → 1, `'B'` → 0

2. **Split the data**
   - 80% training, 20% testing

3. **Standardize features**
   - Using `StandardScaler` to normalize the data

4. **Train Logistic Regression model**
   - Using `sklearn.linear_model.LogisticRegression`

5. **Evaluate the model**
   - Precision Score
   - Recall Score
   - Confusion Matrix
   - ROC-AUC Score

6. **Tune the decision threshold**
   - Manually adjusted threshold to observe its impact on precision

7. **Visualize the sigmoid function**
   - Demonstrates how logistic regression maps inputs to probabilities

---

## Model Evaluation Example Output
- Precision Score: 0.9583 
- Confusion matrix: [[67 2] [ 3 42]]
- Recall Score: 0.9333
- ROC - AOC Score: 0.9648
- for tuned threshold: 0.4, Precision: 0.9459

## 📉 Sigmoid Function

The sigmoid function is used to map any real-valued number into the (0, 1) interval, enabling probability interpretation:

```math
\sigma(z) = \frac{1}{1 + e^{-z}}

The project includes a plot of the sigmoid curve over a range of values.
