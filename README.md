# Analytics Portfolio
**Jovia | MS Business Analytics | University of Houston – Bauer College of Business**  
Supply Chain Analytics | Machine Learning in R | Data Mining

---

## About Me
I am a graduate student specializing in Business Analytics with a focus on supply chain analytics. This portfolio showcases three data mining and machine learning projects completed in R, using real-world datasets sourced from Kaggle. Each project demonstrates end-to-end analytical thinking — from problem definition and data preprocessing to modeling, visualization, and business insights.

---

## Projects

---

### 1. Supply Chain Late Delivery Prediction
**Algorithm:** Random Forest (Classification)  
**Dataset:** DataCo Smart Supply Chain Dataset — Kaggle  
**Libraries:** `tidymodels`, `randomForest`, `ggplot2`, `dplyr`

**Problem Statement**  
Late deliveries are a major operational challenge in supply chain management, leading to customer dissatisfaction and increased costs. This project aimed to predict whether a shipment would be delivered late based on order and shipping characteristics.

**Data**  
The DataCo Smart Supply Chain dataset contains transactional records of orders, products, customers, and shipping details from a global supply chain operation. The dataset required significant preprocessing including handling missing values, encoding categorical variables, and feature selection.

**Data Mining Operations**  
Data was cleaned and wrangled in R using `dplyr`. A Random Forest classification model was built using the `tidymodels` framework. Random Forest was chosen because it handles both categorical and numerical features well, is robust to overfitting, and provides feature importance rankings — valuable for supply chain decision-making. The model was trained and evaluated using cross-validation.

**Model Outputs**  
Feature importance plots identified the most influential variables in predicting late delivery. Confusion matrix and accuracy metrics were used to evaluate model performance. Visualizations were produced using `ggplot2`.

**Limitations**  
The dataset had class imbalance between on-time and late deliveries, which could affect model precision. Some features had missing values that required removal, potentially reducing predictive power. The model's performance may vary when applied to different supply chain contexts or industries.

**Conclusion**  
The Random Forest model effectively identified key predictors of late delivery, providing actionable insights for supply chain optimization. The project demonstrated that machine learning can be a powerful tool for proactive logistics management.

---

### 2. House Price Prediction
**Algorithm:** Simple Linear Regression  
**Dataset:** Real Estate Valuation Dataset — Kaggle  
**Libraries:** `ggplot2`, `dplyr`, `base R (lm())`

**Problem Statement**  
Real estate pricing is influenced by many location-based factors. This project aimed to predict house price per unit area based on proximity to the nearest MRT station, testing the hypothesis that transportation access significantly drives property value.

**Data**  
The dataset contained 414 observations of real estate transactions with six independent variables including house age, distance to MRT stations, number of convenience stores, and geographic coordinates. The dependent variable was house price per unit area.

**Data Mining Operations**  
Data preprocessing involved checking for missing values using `is.na()` (none found) and removing outliers using the IQR method, reducing the dataset from 414 to 377 clean rows. Distance to the nearest MRT station was selected as the independent variable based on domain knowledge about transportation's influence on real estate value. A simple linear regression model was trained using `lm()` in R.

**Model Outputs**  
A scatter plot confirmed a clear negative relationship between MRT distance and house price — as distance increases, price decreases. A regression line overlaid on the scatter plot visually confirmed this downward trend. Model coefficients were statistically significant, validating the hypothesis.

**Limitations**  
Using only one independent variable (distance to MRT) limits the model's explanatory power. A multiple regression approach incorporating all six variables would likely produce more accurate predictions. The dataset is also geographically specific and may not generalize to other real estate markets.

**Conclusion**  
The model successfully confirmed that proximity to public transportation is a statistically significant predictor of house prices. The project effectively demonstrated the application of simple linear regression for real estate valuation analysis.

---

### 3. Women's Clothing Reviews — Sentiment Analysis & Word Cloud
**Algorithm:** Sentiment Analysis (Bing & NRC Lexicons) + Word Frequency Analysis  
**Dataset:** Women's Clothing E-Commerce Reviews — Kaggle  
**Libraries:** `tidytext`, `dplyr`, `ggplot2`, `wordcloud`, `syuzhet`

**Problem Statement**  
Understanding how customers feel about products is critical for retail businesses. This project analyzed customer review text to uncover overall sentiment, dominant emotions, and the most frequently discussed topics in women's clothing purchases.

**Data**  
The Women's Clothing E-Commerce Reviews dataset from Kaggle contained written customer reviews. After loading and cleaning the data, stop words were removed and reviews were tokenized into 472,675 individual words. A sample of 5,000 words was used for emotion analysis to improve processing efficiency.

**Data Mining Operations**  
Text preprocessing included tokenization and stop word removal using the `tidytext` package. Sentiment analysis was conducted using two lexicons: the Bing lexicon for positive/negative polarity and the NRC lexicon for multi-class emotion recognition (joy, trust, anger, sadness, etc.). Word frequency analysis and a word cloud were generated to identify the most discussed topics.

**Model Outputs**  
The sentiment analysis revealed that customers are overwhelmingly positive — 74,333 positive words compared to 24,341 negative words, representing approximately 75% positive sentiment. The word cloud showed that the most frequently used words were "dress," "love," and "fabric." The NRC emotion analysis identified positive emotion and trust as the dominant feelings, followed by joy and anticipation.

**Limitations**  
Lexicon-based sentiment analysis does not capture context, sarcasm, or nuanced language. The 5,000-word sample used for emotion analysis may not fully represent the entire dataset. Reviews may also reflect product-specific biases depending on what items were most commonly purchased.

**Conclusion**  
The analysis effectively revealed strong positive customer sentiment toward the clothing brand. The project demonstrated practical text mining techniques applicable to e-commerce, brand management, and customer experience analytics.

---

## Skills Demonstrated
- Machine Learning: Classification, Regression, Text Mining
- Languages & Tools: R, RStudio, tidymodels, ggplot2, tidytext
- Data Wrangling: Missing value handling, outlier removal, feature engineering
- Visualization: Word clouds, scatter plots, feature importance plots, logistic curves
- Domains: Supply Chain Analytics, Real Estate, E-Commerce

---

## Contact
**GitHub:** [JovialAnalyst](https://github.com/JovialAnalyst)  
**University:** Bauer College of Business, University of Houston
