# Trading Algorithm Performance Report 

## Baseline Trading Algorithm 

The Baseline Trading ALgorithm strategy returns are very similar to the actual returns. The model has a high percission; however, the recall is not high. The strategy returns resemble the actual returns; however, in some cases they ar opposite of the actual returns as observed in the ggraph below.  

![Baseline_Trading_Algorithm](Images/Baseline_Trading_Algorithm.png)

## Tuning Baseline Trading Algorithm

### Step 1: Tune the training algorithm by adjusting the size of the training dataset. 

**To do so, slice your data into different periods. Rerun the notebook with the updated parameters, and record the results in your README.md file.
Answer the following question: What impact resulted from increasing or decreasing the training window?**

The training window was increased from 3 months to 9 months. The change miniscullat increased the recall by 0.01 for both outcomes. However, the "1.0" precision dropped by 0.3, but the "-1.0" percision increased by approxiamtely 0.3. The tuned algorithm is not better and the results are similar to the baseline trading algorithm. 

![Tuned_Trading_Algorithm_Part_1](Images/Tuned_Trading_Algorithm_Part_1.png)


### Step 2: Tune the trading algorithm by adjusting the SMA input features.  

**Adjust one or both of the windows for the algorithm. Rerun the notebook with the updated parameters, and record the results in your `README.md` file. 
Answer the following question: What impact resulted from increasing or decreasing either or both of the SMA windows?**

The short window was changed from 4 to 15, and the long window was changed from 100 to 150. As observed in the table below, the percision and recall stats increased all across the board. The changing of the SMA paramteres significnatly improved the performance of the trading algorithm. 


![Tuned_Trading_Algorithm_Part_2](Images/Tuned_Trading_Algorithm_Part_2.png)


### Step 3: Choose the set of parameters that best improved the trading algorithm returns. 

**Save a PNG image of the cumulative product of the actual returns vs. the strategy returns, and document your conclusion in your `README.md` file.**

The graph below is of the modified SMA parameters in step 2 (short window was changed from 4 to 15, and the long window was changed from 100 to 150). 

![Tuned_Trading_Algorithm_Part_3](Images/Tuned_Trading_Algorithm_Part_3.png)


## LogisticRegression  

**Answer the following questions: Did this new model perform better or worse than the provided baseline model? Did this new model perform better or worse than your tuned trading algorithm?**

The percision and recall both increased and decreased for "1.0" and "-1.0" compared to the baseline trading algorithm values. The overall model performance is similar in terms of percision and recall. The overall model accuracy decreased by 0.03. Therefore, the model has slightly poooer performance statistics compared to the baseline algorithm. THe graphs below dispaly these results. 

![LogisticRegression_report.png](Images/LogisticRegression_report.png)

![LogisticRegression](Images/LogisticRegression.png)


## Final Conclusions and Analysis

The baseline model performed fairly well. Most tunings of the model did not result in an improvement in the performance statistics of the trading algorithm. The only modififcation that resulted in a performance improvement was the chanigng of the short and the long windows in Step 2. The graphs in step 2 highlight the improved performance statistics compared ot the baseline model. 


















Did this new model perform better or worse than the provided baseline model? Did this new model perform better or worse than your tuned trading algorithm?