# Readmission Risk in Diabetic Patients

## Project Overview
Hospital readmission is a critical issue in the management of diabetic patients, resulting in significant financial burdens on healthcare systems and highlighting potential lapses in patient care. This project aims to develop a predictive model to assess the risk of hospital readmission for diabetic patients, enabling healthcare providers to take timely interventions and reduce avoidable readmissions.

## Motivation
Traditional approaches to feature selection and classification, such as Chi-square analysis, may overlook complex relationships between features and readmission risk. In this project, we introduce novel enhancements to improve the accuracy of readmission risk prediction models, ultimately benefiting both patient outcomes and healthcare resource management.

## Methodology
Our approach focuses on two primary improvements:
1. **Advanced Feature Selection**: 
   We employ multiple feature selection techniques to better capture the nuances of the dataset:
   - **ReliefF**
   - **Correlation**
   - **Information Gain**
   - **SelectKBest**

2. **Handling Imbalanced Data**: 
   In healthcare data, instances of non-readmission often outnumber readmissions. To address this class imbalance, we apply the **Synthetic Minority Oversampling Technique (SMOTE)** to ensure the robustness and fairness of our models.

3. **Hyperparameter Tuning**: 
   To optimize the model's performance, we use **Grid Search Cross-Validation** to fine-tune classifier parameters, ensuring the best predictive accuracy.

## Dataset
The dataset used in this project contains diabetic patient records, including features such as demographics, clinical metrics, and hospital visit details. The dataset was preprocessed, with SMOTE applied to handle imbalances between readmission and non-readmission cases.

## Models
We tested and optimized various machine learning classifiers using the techniques mentioned:
- Decision Trees
- Random Forests
- Support Vector Machines (SVM)
- Logistic Regression

## Results
By combining advanced feature selection techniques with effective handling of imbalanced data and rigorous hyperparameter tuning, our models achieved improved predictive accuracy in identifying patients at risk of readmission. This could potentially help healthcare providers make more informed decisions and allocate resources more efficiently.

## Installation
To run this project locally:
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/Readmission-Risk-in-Diabetic-Patients.git
    ```
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
1. Preprocess the dataset using the provided preprocessing scripts.
2. Train models using the training script:
    ```bash
    python train.py
    ```
3. Evaluate models and view results:
    ```bash
    python evaluate.py
    ```

## Contributing
Contributions are welcome! Please fork this repository and submit a pull request for any enhancements or bug fixes.

## License
This project is licensed under the MIT License.

## Contact
For any inquiries or issues, please contact [your-email@example.com].
