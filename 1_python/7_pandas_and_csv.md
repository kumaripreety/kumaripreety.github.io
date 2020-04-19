# Pandas And CSV

##### CSV:

- two importnat function [Reader]() and [Writer]()

```python
import csv
F2 = open(r'C:\Users\bh815e\Documents\Personal_Docs\training\assets\dbdump.csv', 'w')
wtr = csv.writer(F2)
wtr.writerow(['IP', 'DATE', 'PICS', 'URL'])
for r in result:
    wtr.writerow(r)
F2.close()
```



##### Pandas:

- Majorly used to process two types of data [DataFrame - 2D]() and [Series - 1D]() 

```python
import pandas as pd
df1 = pd.DataFrame([[10, 20, 30],[40, 50]])
df2 = pd.DataFrame([[10, 20, 30],[40, 50, 60]], index=['r1', 'r2'], columns=['c1', 'c2', 'c3'])

print(df1)
print(df2)
# T - Transpose the data
df3 = df1.T
df3.to_json('out9.json')
df3.to_csv('out9.csv')
df3.to_excel('output.xlsx')
```



- [Adding multiple sheet in excel workbook]()

  

```python
# Create a Pandas Excel writer using XlsxWriter as the engine.

writer = pd.ExcelWriter(r'C:\Users\bh815e\Documents\Personal_Docs\training\assets\Report.xlsx', engine='xlsxwriter')

# Convert the dataframe to an XlsxWriter Excel object.
df4.to_excel(writer, sheet_name='pics_data')

# Get the xlsxwriter objects from the dataframe writer object.
wb = writer.book
ws = wb.add_worksheet('Graph')
ws.insert_image('B2', 'C:\\Users\\bh815e\\Documents\\Personal_Docs\\training\\assets\\graph.png')
writer.close()
```



- [Slicing:]()



```python
# Slicing
# df -- Dataframe
df1 = df.iloc[1,1]		#2nd row , 2nd column
df2 = df.iloc[1]        # 2nd row entire column
# df.iloc[row_start:row_end:jump, column_start:column_end:jump]
df3 = df.iloc[[1, 3, 5], [2, 5, 7, 8]]  # 2nd, 4th, 6th row and 3rd, 6th, 8th, 9th column 

```



##### Matplotlib: 

- used to plot and show graph

```python
import pandas as pd
# used to olot graph
import matplotlib.pyplot as plt

df = pd.read_csv('C:\\Users\\bh815e\\Documents\\Personal_Docs\\training''\\assets\\dbdump.csv')
df4 = df['PICS'].value_counts()
print(df4)
df4.plot()
# save graph before show, else data will be lost and empty graph will be saved

plt.savefig(r'C:\Users\bh815e\Documents\Personal_Docs\training\assets\graph.png')
plt.show()
```

