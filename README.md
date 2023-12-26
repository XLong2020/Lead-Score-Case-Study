# Lead-Score-Case-Study**

Lead Score Case Study**

Overview

X Education has tasked us with building a logistic regression model to assign lead scores to potential customers based on their likelihood of conversion. The objective is to target leads more effectively, with a higher lead score indicating a greater chance of conversion. The dataset provided consists of around 9000 data points, including attributes such as Lead Source, Total Time Spent on Website, Total Visits, Last Activity, and more. The target variable, 'Converted,' denotes whether a lead was converted (1) or not (0).

Goals of the Case Study

* Build a Logistic Regression Model:
* Assign lead scores between 0 and 100 to indicate the likelihood of conversion.
* Higher scores suggest a hot lead with a higher chance of conversion, while lower scores indicate a colder lead.
* Adjust to Future Requirements:
* The model should be adaptable to handle future requirements presented by the company.

Results Expected

* Jupyter Notebook:
A well-commented Jupyter notebook containing the logistic regression model, conversion predictions, and evaluation metrics.
* Word Document:
A Word document filled with solutions to problems presented by the company, based on the logistic regression model.
* Presentation:
A concise and clear presentation to showcase the analysis to the chief data scientist. The presentation should cover both technical and business aspects.
* PDF Summary Report:
A brief summary report in PDF format explaining the approach taken in the assignment and key learnings.

Project Flow

* Exploratory Data Analysis (EDA)
Conducted a swift check on null values, removing columns with over 45% missing values.
Handled null values by replacing them with 'not provided' to retain important columns.
Imputed 'not provided' values with 'India,' the most prevalent non-missing value.
Dropped the 'India' column due to its overwhelming prevalence (nearly 97% of the data).
Performed treatment on numerical variables, addressed outliers, and created dummy variables.

* Train-Test Split & Scaling
Split the data into 70% for training and 30% for testing.
Applied min-max scaling to the variables ['TotalVisits', 'Page Views Per Visit', 'Total Time Spent on Website'].

* Model Building
Utilized Recursive Feature Elimination (RFE) for feature selection.
Identified the top 15 relevant variables through RFE.
Manually removed remaining variables based on VIF values and p-values.
Generated a confusion matrix, achieving an overall accuracy of 80.91%.

* Model Evaluation
Sensitivity-Specificity Evaluation
On Training Data: Optimal cut-off value of 0.35 with ROC curve area of 0.88.
Accuracy: 80.91%, Sensitivity: 79.94%, Specificity: 81.50%.
On Test Data: Accuracy: 80.02%, Sensitivity: 79.23%, Specificity: 80.50%.

* Precision-Recall Evaluation
On Training Data: Cut-off of 0.35, Precision: 79.29%, Recall: 70.22%.
After finding the optimal cut-off of 0.44, Accuracy: 81.80%, Precision: 75.71%, Recall: 76.32%.
On Test Data: Accuracy: 80.57%, Precision: 74.87%, Recall: 73.26%.

* Conclusion
Optimal cut-off value for Sensitivity-Specificity Evaluation: 0.35.
Optimal cut-off value for Precision-Recall Evaluation: 0.44.

* Submission Components

** Python Commented File:
Detailed comments and clean code.

** Word File:
Answers to all questions posed by the company.

** Presentation (PDF):
Concise and clear presentation covering technical and business aspects.

** PDF Summary Report:
A brief summary report explaining the assignment approach and key learnings.
