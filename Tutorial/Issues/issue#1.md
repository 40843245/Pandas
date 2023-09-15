# issue1
Q: How to remove index and format output of table without leading whitespace for a dataframe object in pandas in Python?
![image](https://github.com/40843245/Pandas/assets/75050655/ff2ae63d-9a2a-44cb-81e6-d5b433773cd4)

Code:

    import pandas as pd
    
    
    df2 = pd.DataFrame({'Record Type': ['100', '200', '300'],
               'Value': [(1,2,3,4,5), (0,10), 1]},
                index = (['','','']))
    
    print(df2)

I run it in Anaconda Spyder console. 

And I expect it displays.

    Record Type            Value
            100  (1, 2, 3, 4, 5)
            200          (0, 10)
            300                1
However, it displays with a leading whitespace.

     Record Type            Value
         100  (1, 2, 3, 4, 5)
         200          (0, 10)
         300                1

Although I have google it and find API of pandas, I just find a way to achieve it -- set the index as empty string ''.

Any replies will be helpful.

I post it in stackoverflow and Github.

stackoverflow:

https://stackoverflow.com/questions/77109581/q-how-to-remove-index-and-format-output-of-table-without-leading-whitespace-for

Github:

https://github.com/40843245/Pandas/blob/main/Tutorial/Issues/issue%231.md
