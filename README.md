# python-
import pandas as pd
import numpy as np

a = pd.read_excel('zoo.xls')

a.head(3)
a[:3]

a[['animal','age']]

a.loc[['d','e','i'],['animal','age']]

a[a.age>3]

a[a.isnull().values==True]

(a[a.age>2])[a.age<4]

a.loc['f','age'] = 1.5

sum(a.visits)

a.groupby('animal').mean()

a.animal.value_counts()

a.replace(['yes','no'],[True,False],inplace=True)

a.replace('snake','python')
