split multiplier approaches
-will reprice stock after downloading
1)convert prices to a list and reverse iterate through this list, multiplying
by appropriate split product.

2)figure out how to do the multiplying in pandas.
    a. first create a new "multiplier" column
       -use df.cumprod() pandas dataframe operator to get the cumulative product 
       -determined by date range
    b. next, create a new "real price" column from the product of
       the "multiplier" column and the original "Close"
