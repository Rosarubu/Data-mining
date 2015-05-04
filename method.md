deal with claims data    


Filter : drop the missing data from PCP, ProviderID, Vendor     
Metadata:   change MemberID to rejected, 




Impute : Class/Interval Variables impute method: Tree      
Indecator type:Unique       
Role:Input    

Note: The GLM Role values Model and ZI Model and ZI Model are specific when modeling a Zero-Inflated Poisson (ZIP) model or Zero-Inflated Negative Binomial (ZINB) model and the ZI Model Variables property is set to User Defined. A zero-inflated model is typically used to predict claim counts. It is normal for insurance data to contain a large proportion of observations that have zero values for claim count variables. The zero-inflated approach fits two separate models, and then combines them. First, a logit model is fit to determine whether an observation contains a zero count claim variable, or not. Then a Poisson or negative binomial model is used to fit observations with nonzero values for the claim count variables (claim counts of 1, 2, 3, and so on.) The two models are then combined.







                                            Number
Data                                          of                                Mode                            Mode2
Role     Variable Name             Role     Levels    Missing    Mode        Percentage    Mode2              Percentage
 
TRAIN    MemberID                 INPUT       513          0     1027829        0.67       1060508               0.67
TRAIN    PCP                      INPUT       513        150     91972          3.12       20893                 1.95
TRAIN    PlaceSvc                 INPUT         9        231     Office        57.88       Independent Lab      23.94
TRAIN    PrimaryConditionGroup    INPUT        46        340     MSC2a3        17.79       METAB3               12.70
TRAIN    ProcedureGroup           INPUT        18        132     EM            39.37       PL                   18.08
TRAIN    ProviderID               INPUT       513          8     7053364       11.87       1076052               6.18
TRAIN    Sex                      INPUT         3      35185     F             38.43                            35.19
TRAIN    Specialty                INPUT        13        340     Internal      24.61       Laboratory           23.75
TRAIN    Vendor                   INPUT       513         47     240043        10.76       140343                7.34
TRAIN    daysinhospital           TARGET       16          0     0             72.61       1                     9.62
 

Data Role=TRAIN
 
                                        Standard          Non
Variable           Role         Mean    Deviation     Missing     Missing     Minimum      Median     Maximum    Skewness    Kurtosis
 
AgeAtFirstClaim    INPUT    61.68137    20.46548        89840       10160           9          69          80    -1.09485    0.249321
CharlsonIndex      INPUT     1.06417    1.076877       100000           0           0           2           5    0.293584     -0.9495
DSFS               INPUT    145.1931    103.1572       100000           0           0         120         360    0.384104    -1.14533
LengthOfStay       INPUT     0.04812    0.726216       100000           0           0           0          56    50.13224    3268.929
PayDelay           INPUT    43.86197    33.08874       100000           0           0          34         162    1.988395    4.014812
drugcount          INPUT     1.94768    2.142417       100000           0           0           1           7    0.934135    -0.22392
labcount           INPUT     2.42268    3.007343       100000           0           0           1          10    1.109929    0.089299
 
