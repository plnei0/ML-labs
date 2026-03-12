##  Lab 5 – Feature Engineering and Model Experiments

In this lab, I worked with a food delivery dataset to perform feature engineering and evaluate
how different modifications affect the machine learning model

The original notebook code was kept unchanged and all task implementations were added at the end of the original file. 

" For each task I included a short explanation directly under the code."

### Task 1 – Creating a New Feature

I created a new feature called `delivery_speed` by dividing the delivery distance by the delivery duration.
This feature represents how fast the delivery was completed and may influence the order status prediction.

### Task 2 – Modifying Peak Hour Rule

I experimented with a different rule for `is_peak_hour` by defining peak hours between 11 AM and 10 PM based on the order time. 
After retraining the model the performance remained almost the same.

### Task 3 – Changing `top_k` for Item Reduction

I tested different values of `top_k` (10, 30, and 50) when reducing the `Item_Name` feature
Since the dataset contains only a small number of unique item names 
changing `top_k` did not significantly affect the accuracy or the top feature importances

### Task 4 – Feature Selection

I ran the optional feature selection section using `SelectFromModel`
The model accuracy remained nearly the same
which indicates that feature selection did not significantly improve the model performance in this case.

### Notes

All task implementations were added below the original notebook code, and each task includes a short explanation directly under the implemented code cells.
