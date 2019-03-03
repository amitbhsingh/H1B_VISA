
# <b style="color:red; font-family: Babas; font-size: 2em;"> H1B_VISA  </b>



#### This Project is an attempt to simplify the immigration process

#### I will try to update the work as frequantly as I can

# Here the goal
### Is we are tying make a predictive model that can possibly predict the outcome as if and individual applicant of H1B_VISA is Approved or Declined based on given features i.e information he has provided while filling the form for immigration

## Exploration with visuals and aggregation to better understand data:
* Total of Visa Certified and Denied plotting and numerical glimpse
* Top 10 Employers
* Acceptance rate of the Companies or let's say brand names 

## To Do List
### Cleansing & Transformation:
*  We are going get rid of redundant columns as in country we only have all United states of America and the missing values in that column were also USA 

* Reason for removing Employer Province as we have another column which is called EMPLOYER STATE which is same as province EMPLOYER_PROVINCE

*  Changing the Target variable: CASE_STATUS to 0 and 1 
 
*  Date Transformation: All the dates are in string format which we would like to convert into date

* We would like to see the difference of date that is employment starting date and employment end date. 

* We would like to see the processing time of decision making 

* We will add a new column for each employment duration and processing time

* Adjust the WAGE_UNIT_OF_PAY has different levels  'Year', 'Hour', 'Week', 'Bi-Weekly', 'Month', nan. And that is why we need to convert income in one standard we will try converting all in Year format 
* We are going to manually select all the categorical value and encode them to numeric form




# Modeling
## Train and Test split excluding the float and Timedelta due to error in python.  
## Adding features one by one to test if the modeling is improving/ Baseline model is working now with few variables it is giving 58 % Accuracry
## Parameter tunning improved the accuracy to 62 percent 
## lol 100 Percent with Xgboost which is unreal and unbelievable. But curious to find out the reason 
## _kfrold cross validation with  Accuracy: 99.98% (0.07%) Still I am skeptical  and I would like to cross verify the results_
