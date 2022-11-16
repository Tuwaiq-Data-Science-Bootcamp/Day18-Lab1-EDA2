
# Spearmans Rank-Order Correlation:
Spearman’s correlation coefficient (named for Charles Spearman) is a technique used to find the correlation between two data samples. It is available through the Scipy python library.

## Prerequisites: 

   - Data must be ranked
   - Data is preferred to be monotomic (for better results)
   
## Applicability:
  This technique cab be be used on continuous data as long as it is ranked.
  
  
  ![Screenshot_20221116-121706_Chrome](https://user-images.githubusercontent.com/109832303/202139667-9c9d85f2-fe4b-4dea-8c4f-551f5e10ba96.jpg)
  
  
## Is the data suitable or not?
If data is monotonic i.e. decreases together or increases together then yes if not then refer to other methods(Pearson if linear).

![Screenshot_20221116-122102_Chrome](https://user-images.githubusercontent.com/109832303/202140642-db880d1c-f3d1-42a3-9484-d6c2296a13f2.jpg)

## Procedure:
  Assuming we are working with a python pandas dataframe.
  
         - Select 2 columns
         - if data is continuous: 
         - Draw scatterplot to determine if data is monotonic or not
          - If data is monotonic:
               - Rank both columns
               - import Scypy and run the algorithm with those 2 columns as input
         - else refer to another method
   
