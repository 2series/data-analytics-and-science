# The problem
A company wants to automate the loan eligibility process (real time) based on customer detail provided while filling online application form. These details are Gender, Marital Status, Education, Number of Dependents, Income, Loan Amount, Credit History and others. To automate this process, they have given a problem to identify the customers segments, those are eligible for loan amount so that they can specifically target these customers.

# Data
The training set can be found [here](./data/train.csv)  
The test set to validate your model can be found [here](./data/test.csv)
  
| Variable | Description|
|----------|------------|
| Loan_ID  | Unique Loan ID |
| Gender   | Male / Female |
| Married  | Applicant married (Y/N) |
| Dependents | Number of dependents |
| Education | Applicant Education (Graduate/ Under Graduate) |
| Self_Employed | Self employed (Y/N) |
| ApplicantIncome | Applicant income |
| CoapplicantIncome | Coapplicant income |
| LoanAmount | Loan amount in thousands |
| Loan_Amount_Term | Term of loan in months |
| Credit_History | Credit history meets guidelines |
| Property_Area | Urban / Semi Urban / Rural |
| Loan_Status | Loan approved (Y/N) |

# Possible Solution direction and pointers
- Start by getting insights into the data
	- Boxplot
	- Histograms
	- Different types of categories
	- Understand the features (i.e. columns) you have in your data
	- What are numerical statistics e.g. mean, counts, minimal and max values etc..

- Do we have serious missing value problems in our data?
	- Number of NA's
	- How to fill in missing values? ([let me google that for you](https://towardsdatascience.com/how-to-handle-missing-data-8646b18db0d4))
	- Missing values in machine learning ([let me google some more for you](https://towardsdatascience.com/handling-missing-values-in-machine-learning-part-1-dda69d4f88ca))

- Can we draw some conclusions based on random correlations?
	- Does having an education affect yearly income?
	- Does yearly income affect the requested loan amount?
	- Does an education in combination with the requested loan amount affect the approval of a loan?

- What would be a way to predict loan approval based on these data?
	- Feature selection, which columns do you think matter? ([let me google that for you](https://towardsdatascience.com/why-how-and-when-to-apply-feature-selection-e9c69adfabf2))
	- Feature engineering, can you work with the columns present, or do you need to add new ones? ([let me google that for you](https://towardsdatascience.com/understanding-feature-engineering-part-1-continuous-numeric-data-da4e47099a7b))

# How to submit
Create a folder with your name e.g. john-doe inside the solutions folder and put your notebooks inside.
Commit this to your own fork of the data-analytics-and-science repository and create a pull request to the main repository.