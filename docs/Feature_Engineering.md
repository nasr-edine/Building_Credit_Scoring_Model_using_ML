Feature Engineering

1. Dealing with Missing Data:
    - Delete: You could simply delete the rows containing missing when the number of missing value rows count is insignificant (say < 5%)
    - Replace with summary: Summarization here is the mean, mode, or median for a respective column. 
        - For continuous or quantitative variables, either mean/average or mode or median value of the respective column can be used to replace the missing values. 
        - Whereas for categorical or qualitative variables, the mode (most frequent) summation technique works better. 
    - Random replace
    - Using predictive model