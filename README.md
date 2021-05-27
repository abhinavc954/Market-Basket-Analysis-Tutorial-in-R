# Market-Basket-Analysis-Tutorial-in-R
A complete tutorial on Market basket analysis in R, oriented towards practical application.

#Introduction

![image](https://user-images.githubusercontent.com/12694124/119849031-ea46b980-bf29-11eb-8b49-85f27089bb1b.png)

#Terminoloies
Basket & Item Set: Each Basket contains an item set. Eg. If a basket represents a unique Order ID, and 5 distinct items were purchased in that order, then Basket=Order ID and Item Set={i1,i2,i3,i4,i5}.
Metrics for the association rules created { LHS -> RHS }
Support: Fraction of which an item set occurs in our dataset.
      *(Total # of baskets having a particular item set)/(Total baskets in the dataset)
Confidence: probability that a rule is correct for a new transaction with items on the left.      *(Total baskets having both LHS & RHS items of the rule)/(Total baskets that contain LHS items)
Expected Confidence: (Total baskets containing RHS items)/(Total baskets in dataset)
Lift:  (Confidence)/(Expected Confidence). If Lift=1, it means items on LHS and RHS are independent. If Lift>1, means items on LHS & RHS occur together more frequently. If Lift<1, items on LHS & RHS occur together less frequently.
Increment: Confidence – Expected Confidence
Affinity Score:  Lift * Support * Increment *(Avg PricePerUnit of RHS item)
![image](https://user-images.githubusercontent.com/12694124/119849234-17936780-bf2a-11eb-9ae3-6a6689083564.png)

