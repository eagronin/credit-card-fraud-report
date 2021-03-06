# Results

## Overview

This section visualizes and discusses evaluation metrics for the credit card fraud detection models analyzed in the [previous section](https://eagronin.github.io/credit-card-fraud-analyze/).  

This project is based on assignments from Applied Machine Learning in Python by University of Michigan on Coursera.

The analysis for this project was performed in Python.

## Results and Discussion

The precision-recall curve is plotted below:  

![](https://github.com/eagronin/credit-card-fraud-report/blob/master/precision_recall.png?raw=true)

As discussed in an example in the [previous section](https://eagronin.github.io/credit-card-fraud-analyze/), the precision-recall curve shows that the recall of 0.81 can be achieved with a relatively moderate cost in terms of precision, which is 0.95 at such a level of the recall.  This means that the model is effective in predicting fraud (81 percent of fraudulent transactions are identified as such in the test data) with only 5 percent of transactions predicted as fraudulent being predicted incorrectly.

The ROC curve is plotted below:

![](https://github.com/eagronin/credit-card-fraud-report/blob/master/roc.png?raw=true)

As discussed in an example in the 
[previous section](https://eagronin.github.io/credit-card-fraudr-analyze/), it shows that 
the recall (or the true positive rate) of 95 percent can be achieved when the false positive rate is 16 percent.  
However, in this case the precision is going to decline to as low as 7.9 percent (meaning that of all the transactions 
predicted to be fraudulent, only 7.9 percent are indeed fraudulent).

Finally, the figure below draws a heatmap that visualizes the results of the grid search.  As shown in the [previous section](https://eagronin.github.io/credit-card-fraud-analyze/), the best fit for the logistic regression is obtained using L2 penalty and C = 0.062, which falls within the lightest-colored area under L2 of the heat map (i.e., the area corresponding to the highest recall rates).

![](https://github.com/eagronin/credit-card-fraud-report/blob/master/heat_map.png?raw=true)<br/>
Previous step: [Analysis](https://eagronin.github.io/credit-card-fraud-analyze/).
