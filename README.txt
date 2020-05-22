JAMES UKONU
ABSTRACT
DAT 554 Final Project: 
Predictive Analysis on Bank Marketing Data
The bank market telemarketing campaigns requires human expertise and opinions on choosing potential customers. This process takes a lot of time and lacks high level of accuracy. Although, banks today have very detailed customer data as well as transactions and it is expedient to build data driven decisions systems with that will produce high success rate through these campaigns.

Notwithstanding, Machine Learning models and its associated techniques have high tendency to display their influence in solving such problems. 

This project shows how machine learning algorithms can be applied in such practical problem settings, especially with big data sets. The study will showcase case studies I conducted regarding machine learning models in bank marketing campaigns in details while employing different training algorithms. Also, it promises to show simple and useful solutions are provided and discussed. 


I.	INTRODUCTION
This project is about building and optimization of classification models. Essentially, I'm going to do exploratory data analysis and build classification models to predict which client will subscribe to the term deposit and what features have biggest effect on persons decision.
The classification goal is to predict if the client will subscribe a term deposit (variable y). The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed.

II.	DATASET
Source: Kaggle or UCI
Dataset Description:
•	age (numeric)
•	job: type of job (categorical: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown')
•	marital: marital status (categorical: 'divorced','married','single','unknown'; note: 'divorced' means divorced or widowed)
•	education (categorical:'basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown')
•	balance: average yearly balance, in euros (numeric)
•	default: has credit in default? (categorical: 'no','yes','unknown')
•	housing: has housing loan? (categorical: 'no','yes','unknown')
•	loan: has personal loan? (categorical: 'no','yes','unknown')
•	contact: contact communication type (categorical: 'cellular','telephone')
•	month: last contact month of year (categorical: 'jan', 'feb', 'mar', ..., 'nov', 'dec')
•	day_of_week: last contact day of the week (categorical: 'mon','tue','wed','thu','fri')
•	duration: last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.
•	campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)
•	pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted)
•	previous: number of contacts performed before this campaign and for this client (numeric)
•	poutcome: outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success')
•	y - has the client subscribed a term deposit? (binary: 'yes','no') - Output variable (desired target)

It is comprised of 45,211 direct marketing campaigns of a Portuguese banking institution at 3.57MB. The dataset consists of 17 columns with details as shown above.


III.	SOLUTION
This study tends to predict if the client will subscribe a term deposit (variable y) using the provided data with seventeen (17) columns as listed above. Train and test datasets using Machine Learning to build classification models to predict which client will subscribe to the term deposit and what features have biggest effect on persons decision. Also, it will display some exploratory data analysis that will reveal distributions of unique variations contained in the dataset. Models to be used will be Logistic Regression and Decision Trees as discussed with my instructor, Dr. Hei-Chi Chan.

Train these two models on the training set and evaluate each one on the validation set to see which model generalizes best to the unseen data. The test set will be used to provide an unbiased evaluation of the tuned model. The test set is used only once to evaluate the final model. Upon which decision can be made to choose which model provides optimal response from customers.
Models employed were Logistic Regression. Second model employed is Decision Trees upon splitting the Data Frame into testing and training data set and the training the dataset and fitting the pipeline on the dataset.

I initiated the steps shown below:
1.	Exploratory Analysis
2.	Convert Categorical Variables to Number
i.	Label Encoding
ii.	Normalization using Min-Max
iii.	Replacing Variables with Numbers
3.	Data Visualizations
i.	Viewing Statistics and Correlations
ii.	Viewing Outliers
iii.	Using Quartiles and Min-Max Normalization method to resolve Age outlier variables
iv.	Feature Scaling
v.	Dropping NAs
4.	Models Employed:
i.	Logistic Regression
ii.	Decision Trees
5.	Evaluation Metrics-
i.	Area Under Curve (AUC)
ii.	Probability
iii.	Confusion Matrix (Recall, Precision, f1 score)

IV.	EVALUATION METRICS
The evaluation metrics employed were the AUC (Area Under Curve), Accuracy, probabilities and Confusion Matrix whose constituents include: Recall, Precision, f1 score and support. Results showed that the Precision had the best result on the confusion matrix table at 67% under Logistic Regression model and Accuracy performs at 82.7% while AUC shows 85%
On the other hand, the AUC values at 72% under the Decision Trees model and recall metric shows up as precision shows 59% for the confusion matrix outlook.
Also, please note that Decision Trees classifier performed good at different depth as shown in the codes.

V.	CONCLUSION
Obviously, outputs show that value of AUC proves that Logistic Regression classifier performed better then Decision tree classifier in these predictions and that our model is highly prolific for usage in predicting customers’ subscription to the term deposit product of the bank.
ACKNOWLEDGEMENT
First, I want to thank God Almighty for seeing me through this journey at the University of Illinois Springfield. Special thanks go to my friend, big brother, Princeton Anyim for his support through this schooling period. Also, I want to thank my family for their love and support as always.
I want to say a big thank you to my instructors at UIS, they have been very supportive and encouraging. Thank you, Dr. Hei-Chi Chan for your support and for letting me take this course this semester. Honestly, you’ve been amazing.

References
[1]	M. Sergio, C. Paulo and P. Rita, “A data-driven approach to predict the success of bank telemarketing”, a ISCTE-IUL, Business Research Unit (BRU-IUL), Lisbon, Portugal, ALGORITMI Research Centre, Univ. of Minho, 4800-058 Guimarães, Portugal. 
[2]	Z. Chu, “Bank Marketing with Machine Learning”, April 19, 2015. [Online].	 Available:	https://pdfs.semanticscholar.org/a3f6/878eb00901500600a8760046c527e077b33d.pdf
[3]	C. Nelso, “Bank Marketing Campaign Prediction using Logistic Regression”, June 26, 2019. [Online].	Available:	https://medium.com/@ogbeide331/bank-marketing-campaign-prediction-using-logistic-regression-d3a1072ac155
