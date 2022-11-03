# import_Append_All_Sheet_in_One
Import XLS file and Append all sheets in one file

import pandas as pd
df = pd.read_excel(r'C:\Users\RAJG\Downloads\New files Sales data Festive Sale\New_Sheet_7.xls',sheet_name=None)
print(df)

df = pd.concat(pd.read_excel(r'C:\Users\RAJG\Downloads\New files Sales data Festive Sale\New_Sheet_7.xls',sheet_name=None),ignore_index=True)
print(df)

# determining the name of the file
file_name = 'MarksData.xlsx'

# saving the excel
df.to_excel(file_name)
print('DataFrame is written to Excel File successfullyyyyyy.')
