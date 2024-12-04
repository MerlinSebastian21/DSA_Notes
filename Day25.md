# Encoding 
- converting data from one form to another
- Categorical features are generally divided into
    - Binary
    - Ordinal : ordering eg : age (0-3 years)
    - Nominal : names(states,)
 
## One hot Encoding
- datasets may contain columns that has no specefic order of preference
- Label encoding such data may mislead the algorithm

- eg fruits :
- apple,
- orange,
- mango,
- apple -----create columns with distinct fruit values ie
-  apple|Orange|Mango
-  1       0    0
-  0       1    0
-  0       0    1
-  1       0    0

  ## Target Encoding
  - take the statistical data
  ## Frequency Encoding 
  - take value_counts()
  - each category in a categorical variable is replaced with the frequency or count of the category in the dataset

    
 # Feature Scaling

 - It is a technique to standardize the independent feature present in the data in a fixed range
 - Two methods
      - MIN MAX Scaling
      - Standard Scaling
  
## Standard Scaling
- rescales a feature value so that it has distribution with 0 mean value and variance equals to 1
- it follows Standard Normal Distribution(SND)
- Xnew = (Xi -Xmean)/Std dev

 
## MIN MAX Scaling
- rescaling with a distribution value between 0 and 1
- Xnem = (Xi-min(X) )/( max(x)-min(x))
                                                                  
