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
                                                                  
