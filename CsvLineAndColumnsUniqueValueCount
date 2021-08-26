import pandas as pd
import sys

filename=sys.argv[1]
df = pd.read_csv(filename) #===> reads in all the rows, but skips the first one as it is a header.

total_rows=len(df.axes[0]) #===> Axes of 0 is for a row
total_cols=len(df.axes[1]) #===> Axes of 0 is for a column
print("Number of Rows: "+str(total_rows))
print("Number of Columns: "+str(total_cols))

dc = df.groupby('Status')['Id'].nunique()

print (dc)
