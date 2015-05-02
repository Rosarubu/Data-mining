1. replace the categorical variable to numerical. we have *Claims.csv DaysInHospital.csv Labcount.csv DrugCount.csv Members.csv* total 4 tables
  * for *Claims.csv* the variables are listed below __14__ variables include the __LengthOfStay__
  that should be the same with the variable DaysInHospital I assume     
  
     
  MemberID,    
ProviderID,    
Vendor,   
PCP,   
Year, __choose Y2__   
Specialty,   
PlaceSvc,   
PayDelay, __replace the category to number, replace days weeks months  to 1,7,30__    
LengthOfStay,__replace the category to number. replace days weeks months  to 1,7,30 and NULL to 0__   
DSFS,replace the category to number. __replace days weeks months  to 1,7,30 and NULL to 0__   
PrimaryConditionGroup,   
CharlsonIndex,   
ProcedureGroup,   
SupLOS, __choose SupLOS=0 remove =1__ 



at first 2668991 Claims.csv
after the process we have 898873 rows store in Claims_Y2_2.csv    
no of patients(unique row) eq to 71436 Claims_Y2_2.csv 
                     
  * for *DaysInHospital_Y2.csv* only three variables    
  MemberID,    
  ClaimsTruncated,  __leave the untruncated row i.e. remove ClaimsTruncated=1__  
 DaysInHospital    



row no 76039 DaysInHospital_Y2.csv
row no 72067 DaysInHospital_Y2_untruncated.csv
no of patients 72067 in DaysInHospital_Y2_untruncated.csv


  * for *LabCount.csv* for variables
  MemberID,    
 Year, __choose Y2__    
 DSFS,___convert to number___    
  LabCount,__conver to number__

361485 LabCount.csv
after the process 122417 LabCount_2.csv
unique 51269 LabCount_2.csv



  * for *DrugCount.csv* for variables
  MemberID,    
 Year, __choose Y2__    
 DSFS,___convert to number___    
 DrugCount,__conver to number__    
 
 818242 DrugCount.csv
 276028 DrugCount_2.csv
 unique 46213 DrugCount_2.csv



  * for *Members.csv* for variables
  MemberID,     
  AgeAtFirstClaim, __use max__    
  Sex,    
 
113001 Members.csv
unique 113001 Members.csv
