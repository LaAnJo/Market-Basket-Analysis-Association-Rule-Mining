# Market-Basket-Analysis-Association-Rule-Mining
This repository demonstrates Association Rule Mining using a simplified Market Basket Analysis dataset.
Market Basket Analysis – Association Rule Mining
Overview

This repository demonstrates Association Rule Mining using a simplified Market Basket Analysis dataset.
The goal is to analyze customer purchasing behavior and evaluate relationships between items using:

Support

Confidence

Lift

The analysis is based on 500,000 transactions involving three products:

Crisps

Beer

Eggs

Dataset Summary
Item / Combination	Transaction Count
Total Transactions	500,000
Crisps	100,000
Beer	75,000
Eggs	25,000
Crisps & Eggs	20,000
Crisps & Beer	10,000
Beer & Eggs	5,500
Crisps, Beer & Eggs	5,000
Association Rule Metrics

The following standard formulas are used to evaluate association rules:

Support
Support = (Transactions containing all items in the rule) / (Total transactions)

Confidence (A → B)
Confidence = Support(A ∩ B) / Support(A)

Lift (A → B)
Lift = Confidence(A → B) / Support(B)


Lift > 1 → Positive association

Lift = 1 → No association

Lift < 1 → Negative association

Evaluated Association Rules
Rule 1: If Crisps → Beer

Support: 0.02

Confidence: 0.10

Lift: 0.67

📉 Indicates a negative association between crisps and beer.

Rule 2: If Eggs → Crisps

Support: 0.04

Confidence: 0.80

Lift: 4.00

📈 Strong positive association — customers buying eggs are highly likely to buy crisps.

Rule 3: If Beer → Eggs

Support: 0.011

Confidence: 0.0733

Lift: 1.47

📈 Weak but positive association.

Rule 4: If Crisps & Beer → Eggs

Support: 0.01

Confidence: 0.50

Lift: 10.00

🔥 Very strong association — buying crisps and beer together strongly predicts egg purchases.

Rule 5: If Eggs → Crisps & Beer

Support: 0.01

Confidence: 0.20

Lift: 10.00

🔥 Strong association despite lower confidence, indicating a rare but meaningful pattern.

Rule 6: If Eggs & Beer → Crisps

Support: 0.01

Confidence: 0.909

Lift: 4.55

📈 Extremely high confidence — customers buying eggs and beer almost always buy crisps.

Final Summary Table
Rule	Support	Confidence	Lift
If crisps → beer	0.02	0.10	0.67
If eggs → crisps	0.04	0.80	4.00
If beer → eggs	0.011	0.0733	1.47
If crisps, beer → eggs	0.01	0.50	10.00
If eggs → crisps, beer	0.01	0.20	10.00
If eggs, beer → crisps	0.01	0.909	4.55
Key Insights

Eggs act as a strong predictor item, especially when combined with beer.

Crisps + Beer → Eggs shows the strongest association (highest lift).

Some popular items (e.g., crisps → beer) do not necessarily imply strong association.

Use Cases

Retail promotion planning

Product bundling strategies

Recommendation systems

Introductory association rule mining demonstrations
