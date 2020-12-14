import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
dataset = pd.read_csv('groceries.CSV')
transaction =[]
for i in range(0,9835):
transactions.append([str(datasset.values[i,j]) for j in range (0,32)])
from apyori import apriori rules= apriori(transactions,min_support = 0.007, min_confidence = 0.5, min_lift = 3,min_length = 2)
results = list(rules)
dataset.head()
dataset.shape
