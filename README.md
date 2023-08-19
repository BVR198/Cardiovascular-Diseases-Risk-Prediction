# Cardiovascular-Diseases-Risk-Prediction

<div style="padding: 35px;color:white;margin:10;font-size:200%;text-align:center;display:fill;border-radius:10px;overflow:hidden;background-image: url(https://images.pexels.com/photos/3683056/pexels-photo-3683056.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)"><b><span style='color:black'>Getting Started </span></b> </div>

<br>

### 🚀 Getting Started

This project involves analyzing a healthcare dataset with the aim of predicting the prognosis of various diseases. The dataset includes various features related to patients' health and lifestyle, including age, sex, general health, checkup frequency, exercise habits, smoking history, and the presence of various diseases. Each entry represents a unique patient, and the features capture various factors associated with disease prognosis. 💊💡

### 🔧 Tools and Libraries

We will be using Python for this project, along with several libraries for data analysis, machine learning, and data visualization. Here are the main libraries we'll be using:

- **Pandas:** For data manipulation and analysis.
- **Matplotlib and Seaborn:** For data visualization.
- **Scikit-learn:** For machine learning tasks, including data preprocessing, model training, and model evaluation. 🐼📊🔬

### 📚 Dataset

The dataset we'll be using includes various features related to patients' health and lifestyle. Each row represents a unique patient and includes attributes such as age, sex, general health, checkup frequency, exercise habits, and smoking history. The dataset also includes target variables representing the presence of various diseases. 📊💉

### 🎯 Objective

Our main objective is to develop a predictive model that can effectively forecast the prognosis of various diseases based on the provided features. By leveraging the power of machine learning, we aim to enhance the model's accuracy and predictive performance. 📈📉

### 📈 Workflow

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

<br>

![](https://images.pexels.com/photos/1170979/pexels-photo-1170979.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)

<br>

## Domain Knowledge 📚

- **Age**: This is the age of the patient. Age is a crucial factor in disease prognosis as the risk of chronic conditions such as heart disease, cancer, diabetes, and arthritis increases with age. This is due to various factors including the cumulative effect of exposure to risk factors, increased wear and tear on the body, and changes in the body's physiological functions. 🌡️👴

- **Sex**: This feature represents the gender of the patient. Gender can influence disease prognosis due to biological differences and gender-specific lifestyle patterns. For instance, heart disease is more common in males, while skin cancer is more common in females. This could be due to factors like longer life expectancy or different exposure to risk factors in each gender. ♀️♂️

- **General_Health**: This is a self-rated health status of the patient. Patients who perceive their health as "Poor" or "Fair" are more likely to have chronic conditions. This could be because the symptoms or management of these conditions impact their perceived health status. 💓

- **Checkup**: This feature represents the frequency of health checkups. Regular health checkups can help in early detection and management of diseases, thereby improving the prognosis. 🏥

- **Exercise**: This feature indicates whether the patient exercises regularly or not. Regular exercise can help control weight, reduce risk of heart diseases, and manage blood sugar and insulin levels, among other benefits. This aligns with the negative correlation observed between exercise and diseases such as heart disease, diabetes, and arthritis. 🏃‍♂️🏋️‍♀️

- **Smoking_History**: This feature indicates whether the patient has a history of smoking. Smoking can increase disease risk as it can damage blood vessels, increase blood pressure, and reduce the amount of oxygen reaching the organs. 🚬🚭

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



<br>

### <b>I <span style='color:#FF8551'>|</span> Import neccessary libraries</b>

# <span style="color:#E888BB; font-size: 1%;">EXPLORATORY DATA ANALYSIS</span>
<div style="padding: 35px;color:white;margin:10;font-size:170%;text-align:center;display:fill;border-radius:10px;overflow:hidden;background-image: url(https://images.pexels.com/photos/3683056/pexels-photo-3683056.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)"><b><span style='color:black'>EXPLORATORY DATA ANALYSIS </span></b> </div>

<br>

<div style="display: flex; flex-direction: row; align-items: center;">
    <div style="flex: 0;">
        <img src="https://images.pexels.com/photos/4021808/pexels-photo-4021808.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="Image" style="max-width: 300px;" />
    </div>
    <div style="flex: 1; margin-left: 30px;">
        <p style="font-weight: bold; color: black;">Diving into Disease Prognosis</p>
        <p>This project puts a spotlight on the <b><mark style="background-color:#FCE38A;color:white;border-radius:5px;opacity:1.0">Healthcare Dataset</mark></b>, aiming to identify key patterns and factors associated with various diseases. With an application of techniques such as <b><span style='color:#FCE38A'>univariate</span></b>, <b><span style='color:#FCE38A'>bivariate</span></b>, and <b><span style='color:#FCE38A'>multivariate analysis</span></b>, we endeavor to unravel complex relationships and significant determinants in the dataset.
        </p>
        <p style="border: 1px solid black; padding: 10px;">Our exploratory data analysis reveals insightful patterns and trends related to the occurrence of diseases. However, while interpreting these findings, it's crucial to remember the difference between correlation and causation. It is important to note that our exploratory analysis, though comprehensive, does not establish a causal relationship between the features and disease occurrences.
        </p>
        <p style="font-style: italic;">Let's embark on this exploratory journey to extract valuable insights from our data. Ready for the deep dive? 🧐🔍
        </p>
    </div>
</div>

<br>


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

