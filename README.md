# Detecting-phishing-websites-using-ML

This project is based on a problem mentioned in the Goa Police Hackathon 2024, where the objective was to detect and categorize websites as phishing or legitimate. While we didn't participate in the hackathon, we took this topic and worked on it independently to build a machine learning model to classify websites.

### Project Overview

The goal of this project is to build a machine learning model that detects phishing websites using a variety of features derived from the URLs and domains. The dataset was imbalanced, which was addressed by balancing the data for improved classification performance. The project includes an analysis of the data, training of various machine learning models, and a user-friendly function to predict whether a website is phishing or legitimate.

### Dataset

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

### Methodology

