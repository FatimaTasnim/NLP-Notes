To find the accuracy
```Python
import numpy as np
lr_predicted = text_lr_clf.predict(twenty_test.data)
lr_clf_accuracy = np.mean(lr_predicted == twenty_test.target) * 100.

print(f'Test Accuracy is {lr_clf_accuracy}')
```

# Confusion Matrix 
Calculate the test accuracy to find out the Confusion Matrix
```Python
from sklearn.metrics import confusion_matrix
cf = confusion_matrix(y_true=twenty_test.target, y_pred=lr_predicted)
print(cf)
```

This prints a giant list of numbers which is not very interpretable. Let's try pretty printing this by using the print-json hack

```Python
import json
print(json.dumps(cf.tolist(), indent=2))
```

From the result we can see the matrix size. So, Now we can plot heatmap to visualize the decision tree.

```Python
# this line ensures that the plot is rendered inside the Jupyter we used for testing this code
%matplotlib inline 

import seaborn as sns
import matplotlib.pyplot as plt

plt.figure(figsize=(20,10))
ax = sns.heatmap(cf, annot=True, fmt="d",linewidths=.5, center = 90, vmax = 200)
# plt.show() # optional, un-comment if the plot does not show
```

The result of the above codeblock is following
![Heatmap](heatmap.png)