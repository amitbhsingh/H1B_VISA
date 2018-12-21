
# <b style="color:red; font-family: Babas; font-size: 2em;"> H1B_VISA  </b>




## This Project is an attempt to simplify the immigration process

### I will try to update the work as frequantly as I can

#### Here the goal: is we are tying make a predictive model that can possibly predict the outcome as if and individual applicant of H1B_VISA is Approved or Declined based on given features i.e information he has provided while filling the form for immigration

# To Do List
## Cleansing & Transformation:
*  We are going get rid of redundant columns as in country we only have all United states of America and the missing values in that column were also USA Reason for removing Employer Province aswe have another column which is called EMPLOYER STATE which is same as province'EMPLOYER_COUNTRY''EMPLOYER_PROVINCE'

*  Changing the Target variable: CASE_STATUS to 0 and 1 
 
*  Date Transformation: All the dates are in string format which we would like to convert into date
* We would like to see the difference of date that is employment starting date and employment end date. 
* We would like to see the processing time of decision making 
*  We will add a new column for each employment duration and processing time 
