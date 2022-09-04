# Heart Failure Analysis & Prediction
<p class="text-justify">
Project includes the preliminary analysis and machine learning classifier model for the Heart Failure dataset. Clinical records come from the kaggle collection. The dataset contains columns such as:

* **Age**,
* **Anaemia** - decrease of red blood cells or hemoglobin,
* **Creatinine phosphokinase** - level of the CPK enzyme in the blood (mcg/L),
* **Diabetes** - if the patient has diabetes,
* **Ejection Fraction** - percentage of blood leaving the heart at each contraction,
* **High blood pressure** - if the patient has hypertension,
* **Platelets** - platelets in the blood (kiloplatelets/mL),
* **Serum creatinine** - level of serum creatinine in the blood (mg/dL),
* **Serum sodium** - level of serum sodium in the blood (mEq/L),
* **Sex** - woman or men,
* **Smoking** - if the patient smokes or not,
* **Time** - follow-up period (days),
* **Death Event** - if the patient deceased during the follow-up period.

All features are described on the kaggle page. You can find there everything about this data set. (https://www.kaggle.com/datasets/andrewmvd/heart-failure-clinical-data)
</p>

## Analysis
<p class="text-justify">
I started the preliminary analysis from displaying the data and checking the shape and data types. The next step was verifying all the NaN data. As we have seen, the dataset is free of missing data. Afterwards I decided to copy the original dataset and change all boolean data into strings with the rule: 1 : 'Yes' and 0 : 'No'. Basics statistics and histograms gave us an initial insight into the data. The next step refers to count plots of all boolean data. To this task I used a for loop, which allows to automate the creation of plots. In the results, we can highlight that in the dataset less than 200 men and more than 100 women suffer from cardiovascular diseases. Moreover, about 120 surveyed people suffers from anaemia, about 125 people suffers from diabetes and only less than 100 surveyed people declared himself as a smoker. The pie chart showed that most of the respondents have a proper blood pressure. The establishment of appropriate age groups allowed to probability calculations. A bar chart was prepared on the basis of probability for each group. It points that the risk of heart disease increases with age. In the last step I implemented a histogram with kernel density estimation (KDE) in relation to Death Event column for all numerical columns. The result of this operation is available in the notebook.
</p>
## Classifier model
After the 
