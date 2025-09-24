# Aviation-Social-Media-Propensity-Model
Project focuses on building predictive models to identify customers with high propensity to purchase flight tickets, based on their social media behavior. An aviation company that offers domestic and international travel wanted to move away from broad telemarketing campaigns and adopt a digital targeting approach. By collaborating with a social networking platform, they aimed to deliver personalized advertisements directly to users most likely to buy.

The challenge: Customer purchasing patterns differ by device type (Laptop vs. Mobile). Therefore, two separate models were developed to predict ticket purchase propensity.

## Problem Statement ##
 - The company wanted to apply a targeted digital strategy instead of contacting every customer.
 - Social media data provides insight into user digital and social behavior.
 - Customers’ likelihood of booking varies between laptop users and mobile users.
 - **Requirement:** Build two machine learning models — one for laptop users, and one for mobile users (where any non-laptop device is treated as mobile).

## Dataset Information & Context ##
 - Customer demographics and interaction data from social media.
 - Features included login device type, user activity, engagement metrics, and purchase history.
 - **Target variable:** Propensity to buy flight tickets (binary classification).
 - Data preprocessing was essential due to outliers, missing values, and noise in raw data

## Approach & Methodology $$
1. Data Preprocessing
 - Checked for missing values and imputed appropriately.
 - Identified and handled outliers using the IQR method
 - Scaled numerical features for model compatibility.
 - Encoded categorical variables (e.g., device type, demographics).
 - Split dataset into Laptop subset and Mobile subset for separate modeling.

2. Exploratory Data Analysis (EDA)
 - Analyzed customer activity trends by device type.
 - Correlation checks between social behavior and purchase likelihood.
 - Visualized distribution of propensity scores for laptop vs. mobile users.

3. Model Development
 - Applied classification algorithms such as Logistic Regression, Random Forest, and Gradient Boosting.
 - Built two models:
    - Laptop Model – optimized for behaviors of desktop/laptop users.
    - Mobile Model – optimized for all non-laptop users (smartphones/tablets).
 - Evaluated performance using Accuracy, Precision, Recall, and AUC.

4. Results & Findings
 - Models successfully differentiated customers with high vs. low purchase propensity.
 - Laptop model showed stronger prediction accuracy due to richer user activity data.
 - Mobile model captured a larger volume of users, though engagement patterns were noisier.
 - Both models provided valuable segmentation for targeted ad campaigns.

## Business Impact ##
 - Enabled personalized marketing campaigns instead of broad outreach.
 - Increased conversion rates by focusing ads on high-propensity users.
 - Improved advertising ROI by reducing spend on uninterested users.
 - Gave insights into device-specific behavior, allowing the company to tailor messaging per device.
