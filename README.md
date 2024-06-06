# Mobile Price Range Prediction
![image](https://github.com/Souvik-karmakar/Mobile_Price_Range_Prediction/assets/78291973/0b13b04b-ec79-49d4-8996-139691c00d7b)

## Problem Type :- Classification.
## Problem Statement

In the competitive mobile phone market, companies want to understand the sales data of mobile phones and the factors driving the prices. Mobile phones come in all sorts of prices, features, and specifications, making price estimation a crucial part of consumer strategy. The objective of this project is to identify the relationship between the features of a mobile phone and its selling price. Instead of predicting the actual prices, we classify the price range indicating how high the price is. The dataset contains 2000 records of mobile phone information with 21 features, including both categorical and numerical features.

## Data Description

The dataset consists of 2000 records and 21 features, which include:

- **Battery_power**: Total energy a battery can store in one time measured in mAh.
- **Blue**: Has Bluetooth or not.
- **Clock_speed**: Speed at which the microprocessor executes instructions.
- **Dual_sim**: Has dual SIM support or not.
- **Fc**: Front camera megapixels.
- **Four_g**: Has 4G access or not.
- **Int_memory**: Internal memory in gigabytes.
- **M_dep**: Mobile depth in cm.
- **Mobile_wt**: Weight of mobile phone.
- **N_cores**: Number of cores of the processor.
- **Pc**: Primary camera megapixels.
- **Px_height**: Pixel resolution height.
- **Px_width**: Pixel resolution width.
- **Ram**: Random Access Memory in megabytes.
- **Sc_h**: Screen height of the mobile in cm.
- **Sc_w**: Screen width of the mobile in cm.
- **Talk_time**: Longest time that a single battery charge will last when you are talking over the phone.
- **Three_g**: Has 3G access or not.
- **Touch_screen**: Has a touch screen or not.
- **Wifi**: Has WiFi or not.
- **Price_range**: This is the target variable with values of 0 (low cost), 1 (medium cost), 2 (high cost), and 3 (very high cost).

## Data Exploration

- **Target Variable Distribution**: The classes are almost balanced with each class having around 450 records.
- **Categorical Features**: Most categorical features have similar distributions except for `three_g`, where most phones have 3G access.
- **Numerical Features**: Most numerical features follow a uniform distribution except for `fc`, `px_height`, and `sc_w`, which are right-skewed.
- **Price Range Distribution**:
  - Numerical features like RAM, battery power, `px_height`, and `px_width` increase with price.
  - RAM has the strongest correlation with the target variable, followed by battery power, `px_height`, and `px_width`.

## Approach

1. **Exploratory Data Analysis (EDA) and Feature Selection**:
   - Removed multicollinearity.
   - Selected important features.

2. **Data Splitting**:
   - Split the dataset into training and testing sets.

3. **Model Training**:
   - Trained models on the training set.

4. **Model Evaluation**:
   - Evaluated the performance of the models on the test set.

## Learning Outcomes

Students will gain a better understanding of how variables are linked and how EDA helps in gaining insights about the data. They will learn to classify data into similar groups using Naive Bayes and select important features using Random Forest.

## Repository Contents

- **Data**: Contains the dataset used for the project.
- **Notebooks**: Jupyter notebooks for EDA, feature selection, model training, and evaluation.
- **Results**: Model performance metrics and visualizations.
- **README**: Project overview and details.

## Conclusion

This project demonstrates the process of understanding mobile phone features and their impact on price ranges. By employing techniques like EDA, feature selection, and model training, we can effectively classify mobile phones into different price ranges, aiding in better consumer strategy and decision-making.

