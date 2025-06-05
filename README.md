# KPI-report-Hospital-Performance-Analysis-Power-BI
KPI report: Hospital Performance Analysis ( Massachusetts General Hospital )/MGH

For the Hospital Challenge, As an Analytics Consultant for Massachusetts General Hospital (MGH).
We have built a high-level KPI report for the executive team, based on a subset of patient records. The purpose of the report is to give stakeholders visibility into the hospital’s recent performance and answer the following questions:
•	How many patients have been admitted or readmitted over time?
•	How long are patients staying in the hospital, on average?
•	How much is the average cost per visit?
•	How many procedures are covered by insurance?

In our collection of information, we have details about encounters of different periods, like months and days, where we have a separate encounter ID along with patient ID, the start date of treatment and stop date of treatment, basic encounter cost, total claim, and payers coverage.
We have information related to patients where we have the patient ID along with their name, residential address, and some personal information related to each patient.
Next, we have payers where we have different names of the payers of coverage along with their information.
### In our Report, I provided some conclusions/Findings which will help the hospital to take meaningful insights. 

# Findings: 
1.	To calculate how many patients have been admitted and readmitted over time, we used the count of patient IDs and the distinct count of patient IDs. This gives the total number of patients that is 27891, and out of this total, unique IDs are 974, which is 3.37% of the total patient IDs.
2.	 For calculating how long patients are staying in the hospital on average, I use an average length of stay by using the DAX calculation date-diff in days. Which gives 0.31 days, and if we multiply it by 24 hours, we get 7.34 hours average stay.
3.	For calculating how much is the average cost per visit, we use DAX calculation and calculate the average base encounter cost.
4.	For calculating how many procedures are covered by insurance. Firstly, we created a new table where we collected the information of base encounter cost, patient IDS payers coverage amount, and total claim amount. Filter the payers' coverage amount and remove the zero coverage amount. Then we use a card and perform a DAX  Calculation to calculate the count of payer coverage, which results total number of coverage that is 14305.
5.	Along with these, we also use a matrix table to calculate which patient ID visited the hospital more than once and their are overall repeated ID numbers is 27891.

# Dashboard
![image](https://github.com/user-attachments/assets/0bb33fe2-df09-48d4-8fb9-15b35a0832a7)
