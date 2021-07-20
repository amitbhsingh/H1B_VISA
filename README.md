
# [H1B_VISA Project in jupyter nbviewer](https://nbviewer.jupyter.org/github/amitbhsingh/H1B_VISA/blob/master/h1.ipynb)


# This Project is an attempt to simplify the immigration process

# Abstract:

> *  We are tying to  make a predictive model that can possibly predict the outcome. If an individual applicant of H1B_VISA is Approved or Declined based on given features i.e information he has provided while filling the form for immigration

### Initial exploration with visuals and aggregation to better understand data:
> * [We have given the total of Certified and Denied cases plotting them gives visual idea and numerical glimpse Click to see the project](https://github.com/amitbhsingh/H1B_VISA/blob/master/.ipynb_checkpoints/h1-checkpoint.ipynb)
> * Some of the insights Top 10 Employers. Frequancy of application by companies name gives an idea about which companies experience if applicant has stated in the form has higher chances and also the number of succesful applications.

### Cleansing
> *  We are going get rid of redundant columns as in country we only have all United states of America and the missing values in that column were also USA 

> * Reason for removing Employer Province as we have another column which is called EMPLOYER STATE which is same as province EMPLOYER_PROVINCE

> *  Changing the Target variable: CASE_STATUS from CERTIFIED & DENIED TO 1,0 respectively as we know computers(algorithms) understand numbers better than alpahbets for computation
 
> *  Date Transformation: All the dates are in string format which we would like to convert into date

> * We would like to see the difference of date that is employment starting date and employment end date 

> * We would like to see the processing time of decision making 

> * We will add a new column for each employment duration and processing time

> * Adjust the WAGE_UNIT_OF_PAY has different levels  'Year', 'Hour', 'Week', 'Bi-Weekly', 'Month', nan. And that is why we need to convert income in one standard we will try converting all in Year format 
> * We are going to manually select all the categorical value and encode them to numeric form




### Modeling
> * Train and Test split excluding the float and Timedelta due to error in python.  
> * Adding features one by one to test if the modeling is improving/ Baseline model is working now with few variables it is giving 58 % Accuracry
> * Parameter tunning improved the accuracy to 62 percent 
> *  100 Percent with Xgboost which is unreal and unbelievable. But curious to find out the reason 

* _kfold cross validation with  Accuracy: 99.98% (0.07%) these result is highly unnlikely to be correct_

