# Detecting-phishing-websites-using-ML

This project is based on a problem mentioned in the Goa Police Hackathon 2024, where the objective was to detect and categorize websites as phishing or legitimate. While we didn't participate in the hackathon, we took this topic and worked on it independently to build a machine learning model to classify websites.

### <ins>Project Overview</ins>

The goal of this project is to build a machine learning model that detects phishing websites using a variety of features derived from the URLs and domains. The dataset was imbalanced, which was addressed by balancing the data for improved classification performance. The project includes an analysis of the data, training of various machine learning models, and a user-friendly function to predict whether a website is phishing or legitimate.

### <ins>Dataset</ins>

The dataset used in this project was a combination of the following sources:
1. https://www.phishtank.com/developer_info.php.
2. https://www.kaggle.com/datasets/ndarvind/phiusiil-phishing-url-dataset
3. https://github.com/chamanthmvs/Phishing-Website-Detection/blob/master/raw_datasets/1000-phishing.txt

The final dataset, Final.csv, contains 552,119 websites with labels indicating if they are phishing (1) or legitimate (0). Features extracted from the dataset include:
- URL, URL Length, Digits Count, URL Depth
- URL Entropy, URL Popularity Score
- Domain, Sub-domain Count, Domain Entropy
- Path Length, Special Characters Count
- Has HTTPS, Has IP, Has Suspicious Keywords
- TLD (Top-Level Domain), Has Suspicious TLD
- Label, Target

### <ins>Methodology</ins>

1. Data Preprocessing
   - Combined multiple datasets to form Final.csv.
   - Balanced the dataset to address class imbalance.
2. Exploratory Data Analysis (EDA)
   - Analyzed the distribution of each feature relative to the target (phishing/legitimate).
   - Visualized data and performed statistical analysis.
3. Model Training & Evaluation
   - Trained four classification models: XGBoost, Random Forest, Logistic Regression, Naive Bayes.
   - Stored models and label encoder as .pkl files for future use.
4. Model Comparison
   - Evaluated and compared the performance of each model and generated a comparison table.
5. Website Prediction Function
   - Developed a function that allows users to input a website URL and receive a prediction (phishing or legitimate).

### <ins>Future Work</ins>

- Deployment of the model as a web application.
- Additional feature engineering for model improvement.
- Implementing a real-time prediction system.
  
### <ins>Contributing</ins>

Feel free to fork the repository, open issues, and submit pull requests. Contributions are always welcome!

### <ins>Acknowledgements</ins>

- This project was inspired by a problem mentioned in the Goa Police Hackathon 2024.
- Special thanks to my collaborator, [Disha Savant](https://github.com/Disha-Savant), for working together on this project.
