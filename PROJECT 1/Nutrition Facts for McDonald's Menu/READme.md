# 📊 Fast Food Menu Analysis 🍔

## 📌 Introduction
Fast food is an integral part of modern lifestyles, known for its convenience and taste. However, many consumers are unaware of the nutritional contents of their favorite meals. This report provides an in-depth analysis of McDonald's menu items, examining calorie content, macronutrient distribution, sodium levels, and health implications.

## 📝 Objectives
The primary goals of this analysis include:
- Cleaning and structuring the dataset for analysis.
- Performing Exploratory Data Analysis (EDA) to identify trends and outliers.
- Creating a Healthiness Score to rank items based on nutritional value.
- Analyzing meal combinations to determine overall dietary impact.
- Visualizing key findings to communicate insights effectively.

## 📂 Dataset Description
The dataset used in this analysis consists of nutritional information for McDonald's menu items, with attributes including:
- **Calories**: Energy content per serving.
- **Total Fat & Saturated Fat**: Indicators of unhealthy lipid content.
- **Trans Fat & Cholesterol**: Linked to cardiovascular risks.
- **Sodium**: A major contributor to hypertension.
- **Carbohydrates & Sugars**: Significant factors in energy balance and metabolic health.
- **Protein & Fiber**: Essential for muscle maintenance and digestion.
- **Vitamins & Minerals**: Micronutrient contributions to overall health.

## 🔍 Data Cleaning & Preprocessing
Before analysis, several steps were undertaken:
- **Handling Missing Values**: Checked and confirmed data completeness.
- **Standardizing Serving Sizes**: Extracted numerical values from the ‘Serving Size’ column.
- **Creating New Features**: Added ‘Calorie Density’ and ‘Healthiness Score’ for deeper insights.

## 📊 Exploratory Data Analysis (EDA)
### 1️⃣ Calorie Density Analysis
- **Highest Calorie Item**: Chicken McNuggets (40-piece) with 1880 kcal.
- **Lowest Calorie Item**: Water and Diet Coke (0 kcal).
- **Calorie Density Metric**: Evaluated calorie content per gram and milliliter.

### 2️⃣ Sodium & Sugar Levels
- **Excess Sodium**: Some items exceed 3600mg of sodium, surpassing daily recommended limits.
- **High Sugar Content**: Beverages significantly contribute to excessive sugar intake.

### 3️⃣ Healthiness Score Calculation
A weighted scoring system was used:
```
( Calories/2000 * 0.4 ) + ( Sodium/2300 * 0.4 ) + ( Sugar/50 * 0.2 )
```
- **Healthiest Items**: Water & unsweetened beverages (Score: 0.0).
- **Unhealthiest Item**: 40-piece McNuggets (Score: 1.01, exceeding daily limits).

### 4️⃣ Meal Combination Analysis
| Meal | Total Calories | Total Sodium (mg) |
|------|--------------|------------------|
| Big Mac + Large Fries + Large Coke | 1350 kcal | 1440 mg |
| Grilled Chicken Sandwich + Side Salad + Water | 390 kcal | 800 mg |

## 📈 Key Visualizations
- **Top 20 highest and lowest calorie items**
- **Calories vs. Macronutrients (Protein, Fat, Carbs)**
- **Crispy vs. Grilled items: A comparative analysis**
- **Caloric distribution of beverages vs. other food categories**
- **Correlation between sodium and calorie content**

## 🚀 Key Findings & Insights
- **Excessive Sodium & Calories**: Many fast food items surpass daily nutritional recommendations.
- **Grilled Options Are Healthier**: Grilled items generally contain lower fat and calorie levels than crispy options.
- **Hidden Sugars in Beverages**: Soft drinks and shakes contribute disproportionately to sugar intake.
- **Meal Choices Impact Health**: Selecting balanced meals significantly reduces dietary risks.

## 🛠️ Recommendations
- **Health-Conscious Choices**: Opt for grilled items, salads, and water.
- **Sodium Awareness**: Avoid high-sodium meals or balance intake with low-sodium alternatives.
- **Limit Sugary Beverages**: Replace sodas with healthier alternatives like unsweetened drinks.
- **Portion Control**: Be mindful of serving sizes to prevent excessive calorie intake.

[**Full Report**](https://github.com/raymanwaytt/OIBSIP/blob/master/PROJECT%201/Nutrition%20Facts%20for%20McDonald's%20Menu/Fast%20Food%20Menu.ipynb)

## 📢 Conclusion
This project provides critical insights into fast food nutrition, empowering consumers to make informed dietary decisions. By leveraging data analytics and visualization, we can demystify menu items and encourage healthier eating habits.

---
📧 [**Contact**](mailto:arunaabdulrahman01@gmail.com) | 🔗 [**LinkedIn**](http://linkedin.com/in/abdulrahman-aruna-4b564b327)