# D212-Association-Rules-and-Lift-Analysis
## Libraries
* pandas
* numpy
* matplotlib
* mlxtend(preprocessing, frequent_patterns)

## Research Question
Are there relationships of purchased prescriptions?  Are there tendencies that patients whom buy one prescription are likely to buy another prescription? 

My goal is to learn the purchasing tendencies of patients to determine which products they are likely to buy based on previous purchase history. 
 
## Market Basket Justification
This market basket analysis would help determine the chances of a patient to purchase a medication if they previously purchased another medication.  I used the following 3 metrics to measure these associations which are Support, Confidence, and Lift (Maitra, 2019). 
•	Support – contains details about frequently bought items
•	Confidence – indicates how often items are bought together.
•	Lift – “indicates the strength of a rule over random over random occurrence” (Maitra, 2019).
I expect applying the apriori algorithm to the data set will help identify purchasing relationships. 

As one example, I visually identified a purchasing relationship between “bilify” and “paraxeline”.  These two drugs are sometimes purchased together. 

One assumption of market basket analysis is multiple medications are often prescribed for the same condition.  Market basket analysis will help identify these relationships. 

## Data Summary and Implications

The support metric indicates the relative concentration of a drug in the dataset.  Values must be higher than zero to be considered significant.  The top three support values for this analysis follow:

![image](https://user-images.githubusercontent.com/46407407/187062053-9e4694b1-4b0b-4475-944e-bc2d4766fa55.png)

The lift metric measures the tendency two (or more) items are sold together.  Values must be higher than one to be considered significant.  The top three lift values follow:
![image](https://user-images.githubusercontent.com/46407407/187062079-39fd0e36-53fb-4873-bf04-22d325de2392.png)

The confidence metric measures how often the purchase of the antecedent is tied to the consequent.  Confidence displays the probability the consequent will be purchased if the antecedent has been purchased.  The top three confidence values follow:
![image](https://user-images.githubusercontent.com/46407407/187062110-6d74b175-c034-4a57-a297-1a727378a2f4.png)

The practical significance of this analysis is we are now able associate numeric metric on lift, confidence, and support.  This will allow the ability to target and create purchasing incentives for the strongest relationships. 

A course of action for an organization would be to find the linking of purchase items and then try to increase sales based on this information.  One such example is the drug Carvedilol is the consequent for the second and third highest lift values, for Lisinopril and Glipizide respectively. Somehow incentivizing Carvedilol may increase sales of Lisinopril and Glipizide. Incentives could include price reductions and sending marketing material and samples to doctor offices. 

## Sources - Code
1. Kesselly Kamara (April, 2022). Data Mining II.
https://wgu.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=5aefcf2b-73cd-41f5-b4d3-aea0011efd05
(Kamara, 2022)

2. Sarit Maitra (Oct 15,2019). Association Rule Mining using Market Basket Analysis.
https://towardsdatascience.com/market-basket-analysis-knowledge-discovery-in-database-simplistic-approach-dc41659e1558
(Maitra, 2019)


## Sources - Inline
1. Sarit Maitra (Oct 15,2019). Association Rule Mining using Market Basket Analysis.
https://towardsdatascience.com/market-basket-analysis-knowledge-discovery-in-database-simplistic-approach-dc41659e1558
(Maitra, 2019)
2. Jihargifari (Aug2, 2020). How To Perform Market Basket Analysis in Python
https://medium.com/@jihargifari/how-to-perform-market-basket-analysis-in-python-bd00b745b106
(Jihargifari, 2020)

