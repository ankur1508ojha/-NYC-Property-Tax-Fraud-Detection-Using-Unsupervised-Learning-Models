# -NYC-Property-Tax-Fraud-Detection-Using-Unsupervised-Learning-Models
# Overview
This project focused on detecting potential tax fraud from over 1 million NYC property records. By leveraging advanced unsupervised machine learning techniques, we aimed to uncover anomalies and unusual property valuations indicative of fraudulent activity.
# Data Source
The Property Valuation and Assessment Data of New York City were obtained from the NYC Open Data website.
The data can be found here: https://data.cityofnewyork.us/Housing-Development/Property-Valuation-and-Assessment-Data/rgy2-tti8

# Dataset
Total records: 1M+
Features: 32 original variables from NYC property records
# Data Processing and Preprocessing
   Data Analysis & Cleansing : Visualized 32 variables to understand distributions. Many variables showcased a right-skewed distribution, handling skewness with appropriate transformation techniques.
   Imputation:  Innovatively imputed missing values based on data distribution insights.
# Feature Engineering
   Added 45 new variables, primarily focusing on property size and value assessment.
   Normalized property value variables by three size variables, resulting in nine significant variables.
   Grouped averages were calculated based on different categories, resulting in the final 45 variables.

# Machine Learning Techniques Applied
  Dimensionality Reduction: Used PCA to reduce the 45-feature dataset to its most significant components.
  Anomaly Detection: Leveraged a dual-model approach:
  Minkowski-based anomaly detection in the PC space.
  Autoencoder-based detection, focusing on capturing non-linear fraud patterns.
  Unified Fraud Score: Integrated outputs from PCA and the autoencoder to derive a comprehensive fraud score, ranking properties based on this score.

# Data Visualization and Analysis
Heatmap Visualizations: Employed heatmap visualizations to inspect the primary drivers of high fraud scores in top-ranked properties. This provided clarity in understanding which features were most indicative of potential fraud.
Expert Review Preparation: Ranked properties by fraud scores, emphasizing top listings for an in-depth expert assessment.

# Tools & Libraries Used
Machine Learning Library: scikit-learn
Dimensionality Reduction: PCA
Anomaly Detection: Autoencoder, Minkowski distance
Neural Networks: Utilized for training the autoencoder.

# Conclusions
Through this comprehensive approach, we effectively highlighted properties with the highest likelihood of tax fraud. The combination of PCA and autoencoder methodologies provided robust fraud scoring, and heatmap visualizations offered a granular look into the features driving these scores, priming properties for expert evaluation.



