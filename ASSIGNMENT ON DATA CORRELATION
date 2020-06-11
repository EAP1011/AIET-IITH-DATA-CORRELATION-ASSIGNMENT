import pandas as pd
import numpy as np
df=pd.read_csv("houses_to_rent.csv")
df['furniture']=df['furniture'].map({'furnished':1,'not furnished':0})
corr=df.corr(method='kendall')
import seaborn as sns
import matplotlib
matplotlib.rcParams['figure.figsize']=[20,10]
sns.heatmap(corr,xticklabels=corr.columns.values,yticklabels=corr.columns.values,cmap="YlGnBu",annot=True)
