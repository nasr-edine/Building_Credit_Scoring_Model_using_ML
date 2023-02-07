# One Hot Encoder:
- This is a Boolean variable that indicates the presence of a category with the value 1 and 0 for absence.

Example:
Creating dummy variables 

```python
import pandas as pd 
from patsy import dmatrices

df = pd.DataFrame({'A': ['high', 'medium', 'low'],
                   'B': [10,20,30]},
                   index=[0, 1, 2])
print(df)
#----output----
  A      B 
0 high   10 
1 medium 20 
2 low    30

# using get_dummies function of pandas package
df_with_dummies = pd.get_dummies(df, prefix='A', columns=['A'])

print(df_with_dummies)
#----output----
  B  A_high A_low A_medium 
0 10 1.0    0.0   0.0 
1 20 0.0    0.0   1.0 
2 30 0.0    1.0   0.0
