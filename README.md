# Just a script

This script will merge 2 excel into 1 excel. 

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install requirement.

```bash
pip install pandas

```

## Usage
this line will read excel file and specific sheet
```
df1 = pd.read_excel('your_excel_file.xlsx', sheet_name='Data')
```
if you doesn't need specific sheet use this
```
df1 = pd.read_excel('your_excel_file.xlsx', sheet_name='Data')
```

this line will keep the column you need after merge
```
df1 = df1[['Your_column1', 'Your_column2']]
```

when your merge excel file there have a 4 parameter 
- Your excel file name 1
- your excel file name 2
- Parameter for merge
- Type of merge you want to perform. For more documentation [Click here](https://pandas.pydata.org/docs/user_guide/merging.html) 
```
merged_df = pd.merge(df1, df2, on='NPM', how='inner')
```
this code will save the merge excel
```
merged_df.to_excel('Prak2akhir.xlsx', index=False)
```