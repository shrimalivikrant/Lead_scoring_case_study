# Lead_scoring_case_study

PROBLEM STATEMENT :-
An education company named X Education sells online courses to industry professionals. On any given day, many professionals who are interested in the courses land on their website and browse for courses. 
The company markets its courses on several websites and search engines like Google. Once these people land on the website, they might browse the courses or fill up a form for the course or watch some videos. When these people fill up a form providing their email address or phone number, they are classified to be a lead. Moreover, the company also gets leads through past referrals. Once these leads are acquired, employees from the sales team start making calls, writing emails, etc. Through this process, some of the leads get converted while most do not. The typical lead conversion rate at X education is around 30%. 
Now, although X Education gets a lot of leads, its lead conversion rate is very poor. For example, if, say, they acquire 100 leads in a day, only about 30 of them are converted. To make this process more efficient, the company wishes to identify the most potential leads, also known as ‘Hot Leads’. If they successfully identify this set of leads, the lead conversion rate should go up as the sales team will now be focusing more on communicating with the potential leads rather than making calls to everyone. A typical lead conversion process can be represented using the following funnel:
As you can see, there are a lot of leads generated in the initial stage (top) but only a few of them come out as paying customers from the bottom. In the middle stage, you need to nurture the potential leads well (i.e. educating the leads about the product, constantly communicating etc. ) in order to get a higher lead conversion.
X Education has appointed you to help them select the most promising leads, i.e. the leads that are most likely to convert into paying customers. The company requires you to build a model wherein you need to assign a lead score to each of the leads such that the customers with a higher lead score have a higher conversion chance and the customers with a lower lead score have a lower conversion chance. The CEO, in particular, has given a ballpark of the target lead conversion rate to be around 80%.

Methodology:
1. Data Cleaning:
o Addressed null values and irrelevant entries. reclassified
geographical data into 'India', 'foreigner', and 'unknown'.
o Null values were categorized as 'unknown' before being removed
for dummy variable creation.
2. Exploratory Data Analysis (EDA):
o Conducted initial EDA to assess data quality. Identified irrelevant
categories in categorical variables. Confirmed no significant
outliers in numeric data.
3. Dummy Variables Creation:
o Created dummy variables for categorical data. Removed dummies
with 'unknown' entries.
4. Train-Test Split:
o Split the data into 72% for training and 28% for testing.
5. Model Building:
o Used Recursive Feature Elimination (RFE) to select the top 15
relevant variables.
o Manually removed variables with high Variance Inflation Factor
(VIF > 5) and non-significant p-values (p > 0.05).
6. Model Evaluation:
o Constructed a confusion matrix. Determined the optimum cut-off
value using the ROC curve. Achieved an accuracy, sensitivity, and
specificity of approximately 80%.
7. Prediction:
o Applied the model to the test data with an optimum cut-off of 0.35,
maintaining an accuracy of 77% , sensitivity of 86%, and specificity
of 72%.
8. Precision-Recall Analysis:
o Verified results using precision-recall analysis. Identified an optimal
cut-off of 0.41, with precision at 76% and recall at 78%.


List of all files provided:

    Python Notebook "Lead Scoring case.ipynb" : A python file showing code and data analysis
    Lead Score Case Study.pdf : A presentation file
    Assignment Subjective Questions.pdf : Answers to some subjective questions
    Summary.pdf : Summary of the entire case study and its findings.
