# Cardiovascular-Diseases-Risk-Prediction

### `Getting Started`

This project involves analyzing a healthcare dataset with the aim of predicting the prognosis of various diseases. The dataset includes various features related to patients' health and lifestyle, including age, sex, general health, checkup frequency, exercise habits, smoking history, and the presence of various diseases. Each entry represents a unique patient, and the features capture various factors associated with disease prognosis. 💊💡

### Packages Used 

In this project we are using `Python` as a programing language , along with several libraries such as Pandas, Scikit-learn and matplotlib for Data analysis, Machine learning and Data Visualization

- **`Pandas`:** For data manipulation and analysis.
- **`Matplotlib` and `Seaborn`:** For data visualization.
- **`Scikit-learn`:** For machine learning tasks, including data preprocessing, model training, and model evaluation.

### Objective

Our main objective is to develop a predictive model that can effectively forecast the prognosis of various diseases based on the provided features. By leveraging the power of machine learning, we aim to enhance the model's accuracy and predictive performance. 📈📉

###  Workflow

Here's a brief overview of our workflow for this project:

1. **Data Loading and Preprocessing:** Load the data and preprocess it for analysis and modeling. This includes handling missing values, converting categorical variables into dummy/indicator variables, and encoding ordinal variables. 📊🔍🧹

2. **Exploratory Data Analysis (EDA):** Perform exploratory data analysis to gain insights into the dataset, understand the distributions of features, and explore potential relationships between the features and the disease outcomes. 📊🔬📉

3. **Data Cleansing:** Perform data cleansing and transformation to improve the model's performance. This includes imputing missing values and normalizing numeric features. 💡🔬

4. **Feature Engineering :** Creating New Features by applying model knowledge to the features 🧪🔬

5. **Model Training and Validation:** Train the model using a train-test split strategy and make predictions on the test set. 🧪📚🔍

6. **Model Evaluation:** Evaluate the performance of the trained model using appropriate evaluation metrics such as confusion matrix, ROC curve, and Precision-Recall curve, and assess the model's ability to generalize to unseen data using the test set. 📊🔍✅

<div style="border-radius: 10px; border: #DBC4F0 solid; padding: 15px; background-color: #ffffff00; font-size: 100%; text-align: left;">
    🗒️ <b>Note:</b> This workflow provides a structured approach to analyzing the dataset, building a predictive model, and evaluating its performance. By following this workflow, we can gain insights into the dataset, develop an accurate predictive model, and make informed decisions based on the model's predictions. 📊🧪📈
</div>  



<div style="border-radius: 10px; border: #DBC4F0 solid; padding: 15px; background-color: #ffffff00; font-size: 100%; text-align: left;">
    🗒️ <b>Note:</b> These features collectively provide a comprehensive profile of the patient, incorporating demographic factors, health conditions, and lifestyle habits that are all known to influence disease prognosis. The model trained on these features thus has the potential to provide accurate disease predictions based on a wide range of factors. 🧠💡
</div>  

# <span style="color:#E888BB; font-size: 1%;">INTRODUCTION</span>
<div style="padding: 35px;color:white;margin:10;font-size:170%;text-align:center;display:fill;border-radius:10px;overflow:hidden;background-image: url(https://images.pexels.com/photos/3683056/pexels-photo-3683056.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)"><b><span style='color:black'>Introduction</span></b> </div>

<br>
    
## 📝 Abstract

This study presents a detailed examination and modeling of a healthcare dataset with the primary aim of predicting various disease prognoses at the patient level 🎯. The dataset is characterized by a diverse set of features 📊 including `age` 📅, `sex` 👥, `general health` 💓, `checkup` 🏥, `exercise` 🏋️‍♀️, `smoking history` 🚬, and the presence of various diseases like `heart disease`, `skin cancer`, `other cancer`, `diabetes`, and `arthritis` 🦠.

Our exploratory data analysis highlighted significant differences in the distribution of various disease cases, illustrating the impact of various health and lifestyle factors on disease risk. We also encountered missing data in several features, emphasizing the necessity for effective missing data imputation methods 🕵️‍♀️ in healthcare prediction tasks.

We plan to leverage the power of machine learning, specifically gradient boosting algorithms like <b><mark style="background-color:#FCE38A;color:white;border-radius:5px;opacity:1.0">XGBOOST</mark></b> 🚀, to predict disease prognosis. The model will be rigorously trained and validated using a train-test split strategy 🔄, with the aim of delivering remarkable results on several performance metrics.

The disease predictions produced by the model will be evaluated using a confusion matrix, ROC curve, and Precision-Recall curve, providing a comprehensive view of the model's performance 📈. This approach highlights the importance of utilizing multiple evaluation metrics in imbalanced classification tasks ⏳.

This project underscores the potential of machine learning 🧠 in healthcare prediction tasks, providing insights that could aid in patient risk assessment 🗂️, healthcare planning 📝, and strategy formulation in clinical settings 💼. Future work could focus on refining the prediction model 🔍, exploring different strategies for class balancing 🧩, and integrating additional patient data 🔄 to enhance the accuracy and comprehensiveness of disease prognosis predictions 📈.




For the exploratory data analysis (EDA), we will proceed with the following steps:

1. **Univariate Analysis**: We'll inspect each variable individually to understand its distribution and potential outliers. This will provide insights into the characteristics of each variable and help identify any extreme values or anomalies.

2. **Bivariate Analysis**: We'll explore the relationship between each variable and the target variables (`Heart_Disease`, `Skin_Cancer`, `Other_Cancer`, `Diabetes`). This analysis will allow us to understand how each variable is associated with the presence or absence of these diseases. We can use techniques like bar charts to visualize the distributions of the target variables based on different categories or levels of other variables.

3. **Multivariate Analysis**: We'll study the interactions between different variables and how they collectively relate to the target variables. This analysis will help us uncover complex relationships and patterns that may not be apparent in the univariate or bivariate analyses. Techniques such as scatter plots, correlation matrices, and 3D visualizations can be utilized to gain deeper insights into the data.

We'll start with the target variables, and then move on to the other variables. Since the target variables are binary, we can use bar charts to visualize their distributions. 📊🔍


## <div style="padding: 20px;color:white;margin:10;font-size:90%;text-align:left;display:fill;border-radius:10px;overflow:hidden;background-image: url(https://images.pexels.com/photos/3683041/pexels-photo-3683041.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)"><b><span style='color:black'> Univariate Analysis </span></b> </div>

### <b>I <span style='color:#FF8551'>|</span>Numerical Variables</b>

### 🔍 Interpretation of Results:

- 📏 **Height_(cm)**: The height of the patients seems to follow a normal distribution, with the majority of patients having heights around 160 to 180 cm.

- ⚖️ **Weight_(kg)**: The weight of the patients also appears to be normally distributed, with most patients weighing between approximately 60 and 100 kg.

- 📏⚖️ **BMI**: The distribution of Body Mass Index is somewhat right-skewed. A large number of patients have a BMI between 20 and 30, which falls within the normal to overweight range. However, there are also a significant number of patients with a BMI in the obese range (>30).

- 🍺 **Alcohol_Consumption**: This feature is heavily right-skewed. Most patients have low alcohol consumption, but there are a few patients with high consumption.

- 🍎 **Fruit_Consumption**: This feature is also right-skewed. A lot of patients consume fruits regularly, but a significant number consume them less frequently.

- 🥦 **Green_Vegetables_Consumption**: This feature appears to be normally distributed, with most patients consuming green vegetables moderately.

- 🍟 **FriedPotato_Consumption**: This feature is right-skewed. Many patients consume fried potatoes less frequently, while a few consume them more often.

## Bivariate Analysis Result

- `Heart_Disease`:

  - Heart disease is more prevalent in patients who rate their general health as "Poor" or "Fair".
  - It is slightly more common in patients who do not exercise.
  - Males are more likely to have heart disease than females.
  - The prevalence of heart disease increases with age, with it being most common in the 80+ age category.
  - Heart disease is also more common in patients with a history of smoking.


- `Skin_Cancer`:
  - Skin cancer is more prevalent in patients who rate their general health as "Good" or "Very Good".
  - There is not much difference in prevalence based on exercise habits.
  - Females are more likely to have skin cancer than males.
  - The prevalence of skin cancer increases with age, with in being most common in the 70-74 age category.
  - There is not much difference in prevalence based on smoking history.


- `Other_Cancer`:

  - Other cancers are more prevalent in patients who rate their general health as "Poor" or "Fair"
  - They are slightly more common in patients who do not exercise.
  - There is not much difference in prevalence based on sex.
  - The prevalence of other cancers increases with age, with it being most common in the 75-79 age category.
  - Other cancers are more common in patients with a history of smoking.


- `Diabetes`:

  - Diabetes is more prevalent in patients who rate their general health as "Fair" or "Poor".
  - It is more common in patients who do not exercise. 
  - There is not much difference in prevalence based on sex. 
  - The prevalence of diabetes increases with age, with it being most common in the 70-74 age category.
  - Diabetes is more common in patients with a history of smoking.

- `Arthritis`:

  - Arthritis is more prevalent in patients who rate their general health as "Fair" or "Poor"
  - It is slightly more common in patients who do not exercise. 
  - Females are more likely to have arthritis than males. 
  - The prevalence of arthritis increases with age, with it being most common in the 75-79 age category.
  - Arthritis is slightly more common in patients with a history of smoking.


## Multivariate Analysis Results 

### 🔍 Interpretation of Results:

- The distribution of `General Health` by `Age Category` shows that as age increases, the proportion of individuals rating their health as "Good" or "Very Good" decreases, while the proportion rating their health as "Fair" or "Poor" increases.

- The relationship between `General Health` and the disease conditions (`Heart_Disease`, `Skin_Cancer`, `Other_Cancer`, `Diabetes`, `Arthritis`) shows some interesting patterns:

  - For ❤️ `Heart_Disease`, 🦀 `Other_Cancer`, 🩸 `Diabetes`, and 💪 `Arthritis`, the prevalence is higher among those who rate their health as "Poor" or "Fair". This suggests that these conditions may significantly impact individuals' perception of their general health.
  
  - For 🌞 `Skin_Cancer`, the prevalence seems to be more evenly distributed across the different health ratings. This could suggest that skin cancer may not impact individuals' perception of their general health as much as the other conditions.
 
### <b>II <span style='color:#FF8551'>|</span> BMI category</b>

### 🔍 Interpretation of Results:

- The distribution of `BMI Category` by `Exercise` shows that individuals who exercise have a higher proportion of "Normal" BMI, while those who do not exercise have a higher proportion of "Overweight" and "Obese" BMI. This suggests that exercise is associated with healthier BMI levels. 🏋️‍♀️

- The relationship between `BMI Category` and the disease conditions (`Heart_Disease`, `Skin_Cancer`, `Other_Cancer`, `Diabetes`, `Arthritis`) shows the following patterns:

  - For ❤️ `Heart_Disease`, 🩸 `Diabetes`, and 💪 `Arthritis`, the prevalence is higher among those with "Overweight" and "Obese" BMI. This suggests that these conditions may be associated with higher BMI levels.
  
  - For 🌞 `Skin_Cancer` and 🦀 `Other_Cancer`, the prevalence seems to be more evenly distributed across the different BMI categories. This could suggest that these types of cancer may not be as strongly associated with BMI as the other conditions.

### <b>III <span style='color:#FF8551'>|</span> 3D plot: Age_Category, General_Health, and BMI</b>

### 🔍 Interpretation of Results:

- 📊 The 3D plot visualizes the relationship between `Age_Category`, `General_Health`, and `BMI`. The plot shows a wide distribution across all three variables, suggesting a complex interplay between them.

- ℹ️ Please note that the labels for `Age_Category` and `General_Health` are encoded to numerical values for the purpose of 3D plotting, so the exact categories are not directly visible on the axes.


# <span style="color:#E888BB; font-size: 1%;">CORRELATION MATRIX</span>
<div style="padding: 35px;color:white;margin:10;font-size:170%;text-align:center;display:fill;border-radius:10px;overflow:hidden;background-image: url(https://images.pexels.com/photos/3683056/pexels-photo-3683056.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)"><b><span style='color:black'>CORRELATION MATRIX </span></b> </div>

### <b>I <span style='color:#FF8551'>|</span> Data Preprocessing</b>


### 🔍 Interpretation of Results:

- 📊 The correlation heatmap provides a visual representation of the correlation between different features in the dataset. Each square shows the correlation between the variables on each axis. Correlation values range from -1 to 1. Values closer to 1 represent a strong positive correlation, values closer to -1 represent a strong negative correlation, and values around 0 represent no correlation.

- 🔎 Here are some observations from the heatmap:

  - 🩸 `BMI`, `Weight_(kg)`, and `Exercise` have a positive correlation with `Diabetes`. This suggests that individuals with higher BMI and weight or who do not exercise are more likely to have diabetes.
  
  - 😔 `General_Health` has a negative correlation with `Diabetes`, `Heart_Disease`, `Arthritis`, and `Depression`. This suggests that individuals who rate their general health as poor are more likely to have these conditions.
  
  - ❤️ `Age_Category` has a positive correlation with `Heart_Disease`, `Skin_Cancer`, `Other_Cancer`, `Diabetes`, and `Arthritis`. This suggests that the risk of these diseases increases with age.
  
  - ♂️ `Sex_Male` has a positive correlation with `Heart_Disease` and a negative correlation with `Arthritis` and `Skin_Cancer`. This suggests that males are more likely to have heart disease but less likely to have arthritis or skin cancer.
 


### <b>III <span style='color:#FF8551'>|</span> Correlation of each feature with the disease variables</b>

### 🔍 Interpretation of Results:

- 📊 The correlation heatmaps show the correlation of each feature with the five disease variables: Heart_Disease, Skin_Cancer, Other_Cancer, Diabetes, and Arthritis.

- 🔎 From the heatmaps, we can observe the following:

  - ❤️ **Heart_Disease**: This condition shows a strong positive correlation with `Age_Category` and `General_Health`, and a negative correlation with `Exercise` and `Sex_Female`.

  - 🌞 **Skin_Cancer**: This condition is strongly positively correlated with `Age_Category` and `Sex_Male`, and negatively correlated with `Sex_Female`.

  - 🦀 **Other_Cancer**: This condition shows a strong positive correlation with `Age_Category` and `General_Health`, and a negative correlation with `Sex_Female`.

  - 🩸 **Diabetes**: This condition shows a strong positive correlation with `Age_Category`, `General_Health`, and `BMI`, and a negative correlation with `Exercise`
 
  <div style="padding: 20px;color:white;margin:10;font-size:170%;text-align:center;display:fill;border-radius:10px;overflow:hidden;background-image: url(https://images.pexels.com/photos/3683056/pexels-photo-3683056.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)"><b><span style='color:black'>INSIGHTS</span></b> </div>
  

### Age and Disease Prevalence: 🧓👵🏥

The positive correlation between `Age_Category` and the diseases under study aligns with established medical knowledge. It is well known that the risk of chronic conditions such as heart disease, cancer, diabetes, and arthritis increases with age. This is due to various factors including the cumulative effect of exposure to risk factors, increased wear and tear on the body, and changes in the body's physiological functions. ⏳⚕️

### Health Perception and Disease Prevalence: 💓💡

The negative correlation between self-rated `General_Health` and disease conditions underlines the importance of patients' perception of their own health. Patients who perceive their health as "Poor" or "Fair" are more likely to have chronic conditions. This could be because the symptoms or management of these conditions impact their perceived health status. 🩺🔮

### Exercise and Health: 🏃‍♂️🏋️‍♀️💪

The negative correlation between `Exercise` and diseases such as `heart disease`, `diabetes`, and `arthritis` reaffirms the well-established belief in the health benefits of regular physical activity. Regular exercise can help control weight, reduce the risk of heart diseases, and manage blood sugar and insulin levels, among other benefits. 🚴‍♀️🏊‍♂️

### BMI and Diabetes: 🍎🍔🍬

The positive correlation between `BMI` and diabetes aligns with existing knowledge. High BMI, especially obesity, is a known risk factor for type 2 diabetes. Excess fat, particularly if stored around the abdomen, can increase the body's resistance to insulin, leading to increased blood sugar. 🍩📈

### Gender and Disease Prevalence: 👨‍⚕️👩‍⚕️🧬

The correlations between `Sex` and certain diseases reveal interesting patterns. For instance, heart disease is more common in males, which agrees with many studies showing men are at a higher risk of heart disease. Skin cancer, however, is more common in females, which could be due to factors like longer life expectancy or different exposure to risk factors. 🚹🚺

It's important to note that correlation does not imply causation. While these correlations provide valuable insights, they don't tell us whether one variable causes or directly influences another. Further statistical or experimental studies would be needed to determine causal relationships. 📚⚠️🔍

# <span style="color:#E888BB; font-size: 1%;">EDA RESULT & DISCUSSION</span>
<div style="padding: 35px;color:white;margin:10;font-size:170%;text-align:center;display:fill;border-radius:10px;overflow:hidden;background-image: url(https://images.pexels.com/photos/3683056/pexels-photo-3683056.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)"><b><span style='color:black'>EDA RESULT & DISCUSSION</span></b> </div>


### Univariate Analysis: 📊🧪

The distributions of the numerical variables, such as `Height_(cm)`, `Weight_(kg)`, and `BMI`, were mostly normal, with some features like `Alcohol_Consumption`, `Fruit_Consumption`, and `FriedPotato_Consumption` showing a right-skewed distribution. This suggests that a large proportion of patients have low to moderate consumption levels. 🥦🥔🍷

The categorical variables displayed diverse distributions. For instance, most patients rated their general health as "Good" or "Very Good" and had their last checkup within the past year. Moreover, most patients reported exercising regularly, and a majority did not have a history of smoking. 🏥🚭💪

### Bivariate Analysis: 📈👥

The bivariate analysis revealed relationships between selected features and the disease conditions. Diseases like ❤️ Heart_Disease, 🦀 Other_Cancer, 🩸 Diabetes, and 💪 Arthritis were more prevalent in patients who rated their general health as "Poor" or "Fair", did not exercise, and had a history of smoking. 🌞 Skin_Cancer showed a different pattern, being more prevalent in patients with "Good" or "Very Good" general health and not showing a significant difference based on exercise habits. 🚶‍♀️🚶‍♂️

### Multivariate Analysis: 📊🔢

The multivariate analysis showed the interplay between multiple variables. For instance, as age increased, the proportion of individuals rating their health as "Good" or "Very Good" decreased, while the proportion rating their health as "Fair" or "Poor" increased. Similarly, individuals who exercised had a higher proportion of "Normal" BMI, while those who did not exercise had a higher proportion of "Overweight" and "Obese" BMI. 👴👵🏋️‍♂️🏋️‍♀️

### Correlation Analysis: 🧩🔍

Finally, the correlation analysis revealed the strength and direction of the relationships between the features and the disease conditions. `Age_Category` showed a strong positive correlation with all the diseases, indicating that the risk of these diseases increases with age. `Exercise` showed a negative correlation, suggesting that regular exercise may help reduce the risk of these diseases. 💪⏳

<div class="warning" style="background-color: #F8F3D4; border-left: 6px solid #FF5252;font-size: 100%; padding: 10px;">
<h3 style="color: #FF8551; font-size: 18px; margin-top: 0; margin-bottom: 10px;">🚧  Keep in Mind </h3>
Overall, the EDA provided valuable insights that could be instrumental in developing a machine learning model for disease prognosis. It highlighted the importance of features like age, general health, exercise habits, and BMI in predicting the presence of various diseases. However, it's important to note that while these correlations can suggest relationships, they do not imply causation, and further investigation would be necessary to determine causal relationships. 🧬🔬⚖️
</div>







