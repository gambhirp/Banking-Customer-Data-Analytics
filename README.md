## Smarter Banking with Customer Data

### Project Overview

In the modern banking landscape, leveraging customer data is essential for enhancing performance, reducing risk, and delivering personalized services. This project explores the use of demographic, financial, and behavioral data to improve decision-making in credit risk assessment, loan acquisition, and marketing effectiveness. By applying advanced statistical and machine learning techniques, such as logistic regression, random forests, and decision trees, the study uncovers the most influential factors driving customer behavior and credit decisions. Notably, variables such as account balance, past campaign interactions, and call duration emerge as key predictors. The ultimate goal is to build smarter credit assessment pipelines, optimize marketing channels, and improve customer targeting.

The project also investigates several questions central to banking analytics: how customer attributes influence housing loan uptake, how credit risk can be assessed through behavioral patterns, how communication type and timing affect marketing outcomes, and how previous campaign history predicts customer response. These questions guide the analysis and model-building process throughout the study.

### Data Preparation and Methodology

The dataset was cleaned by handling missing values, transforming "unknown" into NA, and converting categorical variables as needed. Outliers were detected using boxplots and removed to ensure model reliability. The 'day' column was grouped into categorical segments, and multicollinearity was assessed through a correlation matrix. After preprocessing, classification models were built using logistic regression, random forests, and decision trees, depending on the research question. The data was typically split into training and validation sets (70/30), and class imbalance was managed using sampling techniques. Random forests were used where non-linear relationships were expected, and logistic regression was applied where interpretability was important.

### Discussion of Findings

The random forest model for housing loan prediction achieved 65.5% accuracy, with a stronger ability to predict negative outcomes than positive ones. Key features included balance, age, and job, which consistently ranked highest in importance using both Gini and accuracy-based metrics. This supports the idea that financial and occupational data are strong indicators of housing loan likelihood.

In the credit risk analysis, the logistic regression model performed better than the decision tree, with higher specificity and AUC (0.8911), indicating better discrimination between creditworthy and risky clients. Duration, month, and housing status emerged as significant predictors, suggesting that both temporal and behavioral features should be considered in risk assessments.

For marketing analysis, the model's AUC score of 0.901 showed excellent prediction capability. Duration of contact was again the most important variable, confirming that more engaged interactions correlate with positive outcomes. The model achieved over 81% accuracy and demonstrated balanced sensitivity and specificity, making it effective for campaign optimization.

Lastly, the fourth analysis using logistic regression showed that customers with successful past campaign outcomes and recent contact history were more likely to engage. Variables like "campaign" (number of contact attempts) had a negative impact when overused, while "previous" and "poutcome" positively contributed to response likelihood. This highlights the importance of timing and prior experience in customer engagement.

### Recommendations

The analysis leads to several practical recommendations. For product development, banks should create differentiated loan offerings tailored to specific demographic and financial profiles. Predictive models should be used to assess credit risk based on behavioral and transactional data. In marketing, sales teams should be trained to maintain longer and more engaging conversations, and campaigns should be scheduled during high-response periods like summer months. Moreover, marketing strategies should be personalized based on customer segments—such as age, balance, and job type—to improve conversion rates.

For client relationship management, banks should focus on re-engaging customers who responded positively in the past and limit contact frequency to avoid fatigue. Segmented follow-up strategies should be employed: offer premium options to high-potential clients, nurture moderately interested ones, and design low-barrier entry points for new or inactive users. These strategies ensure long-term retention and loyalty by respecting customer preferences and maximizing engagement efficiency.

### Conclusion

This project demonstrates the power of customer data analytics in transforming banking operations. By identifying key behavioral and demographic predictors, and applying advanced modeling techniques, the analysis offers a roadmap for optimizing risk management and marketing strategy. The models and recommendations presented here enable banks to not only improve performance metrics but also foster deeper, more personalized relationships with their customers.

