import pandas as pd

#create dataframe 
data = {
    'Gene' : ['BRCA1', 'TP53'],
    'Sample1' : [34.5, 123.5],
    'Sample2' : [23.2, 110.1],
    'Sample3' : [55.1, 98.0]
}
df = pd.DataFrame(data)
print(df)

#create new column for gene expression average
df['Avg'] = (df['Sample1'] + df['Sample2'] + df['Sample3'])/3
print(df)

#Which gene in Sample1 is higher
print(df['Sample1'] > 50)

#create nnew column and print gene expression higher than 50
df['High_Expr'] = df[['Sample1','Sample2','Sample3']].mean(axis = 1) > 50
print(df)

#export pandas to csv file
df.to_csv('gene_expression.csv', index = False)
