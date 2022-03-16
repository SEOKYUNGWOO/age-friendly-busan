# age-friendly-busan

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

train = pd.read_csv('/cotent/sample_data/california_housing_test.csv')
test = pd.read_csv('/content/sample_data/california_housing_train.csv')
train.head()

test.head()
train.describe()

train.hist(figsize=(15,13), grid=False, bins=50)
plt.show()

correlation=train.corr()

plt.figure(figsize=(10,10))
ans.heatmap(correlation, annot=True)
plt.show()

