###Instructions for Isolating Specific Columns of County Health Data

**Getting started:**

Importing numpy and pandas. Run the following codes:
import numpy as np

import pandas as pd

**Defining a data frame:**

 Note that a data frame can be defined as anything. "df" was chosen for simplicity's sake. Run the following code and ensure that the file name is typed in accurately.
 
 df=pd.read_csv('CountyHealthData_2014-2015.csv') 

 **Isolating specific columns:**

Use df.loc function to call up specific columns from the data frame. Ensure that the following code is typed in accurately, otherwise error may occur. Note that any column from the data frame can be called up as long as the name of the column is entered in a way that is consistent with the following format:

df.loc[:,["State","Region","County","Food insecurity","Limited access to healthy foods", "Adult obesity"]]

Note that the "x variable" of the df.loc code input is a colon. This tells colab to only select columns and include all rows.

**Defining the new data set:**

At this point, a new subset of the original data frame has been created. In order to define this subset as a new data frame, define it with the following code. Note that it can be defined as anything: "subset" was chosen for simplicity's sake.

Subset = df.loc[:,["State","Region","County","Food insecurity","Limited access to healthy foods", "Adult obesity"]]

**Exporting the csv file:**

Export the subset defined in the previous step with the following code. Note that "Subset.csv" will be the name of the exported file, and can be anything so long as the format of the code is consitent with the following:

Subset.to_csv("Subset.csv")

Your csv file has now been exported. Happy coding! 





