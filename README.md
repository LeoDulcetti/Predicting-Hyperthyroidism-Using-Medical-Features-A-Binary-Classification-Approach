# Predicting-Hyperthyroidism-Using-Medical-Features-A-Binary-Classification-Approach
**Project Title: Predicting Hyperthyroidism Using Medical Features: A Binary Classification Approach**

### Project Overview

This project develops a binary classification model to predict hyperthyroidism using various medical features. Hyperthyroidism, a condition where the thyroid gland produces an excess of hormones, can lead to a wide range of health issues. Early detection is crucial for effective management and treatment. Given the importance of accurate predictions, this project employs machine learning techniques to enhance diagnostic processes and assist healthcare professionals.

### Dataset

The dataset for this project was imbalanced, containing a larger number of non-hyperthyroid instances compared to hyperthyroid instances. It consists of various medical features deemed relevant for predicting the presence of hyperthyroidism. Due to confidentiality and data privacy, the exact feature details and data source are not disclosed in this public repository.

### Methodology

1. **Preliminary Data Analysis**:
   - Initial exploration of the dataset to understand the distribution of variables, missing values, and preliminary correlations.

2. **Handling Imbalanced Dataset**:
   - Initial model training was conducted on the original imbalanced dataset to establish a baseline performance.
   - Several techniques, including oversampling and synthetic data generation, were applied to balance the classes, which significantly improved model performance metrics.

4. **Model Building**:
   - **Random Forest Classifier**: Chosen for its robustness and effectiveness in handling tabular data.
   - **Hyperparameter Tuning**: Utilized GridSearchCV and RandomizedSearchCV to optimize the model parameters for better performance.

5. **Model Evaluation**:
   - Evaluation based on several metrics, with a focus on recall and AUROC (Area Under the Receiver Operating Characteristic curve) to assess the model's ability to identify positive cases.
   - Initial models on the imbalanced dataset showed lower recall, which improved substantially after balancing the dataset, without compromising the AUROC.

6. **Results**:
   - Post-balancing, the model demonstrated an enhanced recall and maintained an excellent AUROC, indicating a high level of discriminative power between the two classes (hyperthyroid and non-hyperthyroid).

### Technologies Used

- Python
- Libraries: Pandas, Scikit-learn 

### Key Findings

- Balancing the dataset significantly improved the model's sensitivity (recall), which is critical for medical diagnostic tests where missing a positive case (false negative) can have serious health implications.
- The optimized Random Forest model, post-hyperparameter tuning, showed robust performance, making it a reliable tool for predicting hyperthyroidism.
