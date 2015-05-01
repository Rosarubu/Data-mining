1. replace the categorical variable to numerical. we have *Claims.csv DaysInHospital.csv Labcount.csv DrugCount.csv* total 4 tables
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
                     
  * for *DaysInHospital_Y2.csv* only three variables    
  MemberID,    
  ClaimsTruncated,  __leave the untruncated row i.e. remove ClaimsTruncated=1__  
 DaysInHospital  
