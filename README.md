### M12_CHALLENGE

# CREDIT RISK RESAMPLE

## OVERVIEW

The threat of bias is a constant in Machine Learning models. In an effort to optimize results, these models can ironically, undermine their own efficacy by learning to analyze and predict certain elements too well, to the detriment of the other components that are present within a compilation of data. In an effort to alleviate the effects of the Imbalanced Classes, this module will display the power of Supervised Learning in coordination with the Oversampling technique to analyze Healthy and High Risk lending data to predict the frequency of credit risk. This project will accomplish the following:

1. Split the data into training and testing sets.

2. Create a Logisitic Regression Model with the original lending data.

3. Predict a Logisitic Regression Model with Resampled training data.

4. Write a Credit Risk Analysis Report.

## TECHNOLOGIES

In order for this supervised learning module to run, there are installation requirements. They are the following:

[Python](https://www.python.org/downloads/) - Enables the user to use the powerful Python programming language.

[JupyterLab](https://jupyter.org/) - Access to the web-based IDE JupyterLab.  

[Pandas](https://pandas.pydata.org/) - Grants access to the open-source Pandas data analysis tool, which is powered by Python.

[Scikit-Learn](https://scikit-learn.org/stable/install.html) - Provides users with a library of tools for predictive data analysis.

[Imbalanced-Learn](https://imbalanced-learn.org/stable/) - A library that works in conjunction with scikit-learn, Imbalanced-Learn uses tools to deal with classification with imbalanced classes.

[Microsoft Excel](https://www.microsoft.com/en-us/microsoft-365/excel) - Enables the user to read compiled historical lending data.


## USAGE

In order to execute this Supervised Learning model, you must run the following:

```python
credit_risk_resampling.ipynb
import numpy as np
import pandas as pd
from pathlib import Path
from sklearn.metrics import balanced_accuracy_score, classification_report
from sklearn.metrics import confusion_matrix
from imblearn.metrics import classification_report_imbalanced

import warnings
warnings.filterwarnings('ignore')
```

Accessing JupyterLab in Bash: `Jupyter Lab`

## ANALYSIS REPORT

After the analysis of the lending data using Logistic Regression on the original set and the resampled set, the conclusion is represented in the following metrics:

**Logistic Regression (Original Data)**

* Balanced Accuracy Score: 95.2%
    
    **Healthy Loans:**
        
      * Precision: 100%

      * Recall: 99%
    
    **High Risk Loans:**
    
      * Precision: 84%

      * Recall: 99%

**Resampled Logistic Regression**

* Balanced Accuracy Score: 99.4%

    **Healthy Loans:**
    
      * Precision: 100%

      * Recall: 99%

    **High Risk Loans:**

       * Precision: 85%

       * Recall: 91%

As you can see, based on these metrics, resampling the data does have an effect on the ratios on the imbalanced data set, which in this case is the High Risk Loans. The Precision of the original dataset compared to the resampled dataset is an increase of one percent. However, the Recall of the original decreases by 9% in the resampled instance. In the case of the Healthy Loans, the results are identical. Given that the results of the model are predicted at such a high ratio in both instances there is not a significant enough change to warrant resampling the data. xI would be very interested to see what effect undersampling the data would have had since there was such a massive difference between the instances of Healthy Loans and High Risk Loans. 


## GALLERY


## CONTRIBUTORS

*Marcus LeGare (Author, Developer)*

### LICENSE

**COLUMBIA UNIVERISTY FINTECH BOOTCAMP**