0 missing values across all 12 columns.
0 exact duplicate rows.
5,000 unique order IDs.
989 unique customers.

"I validated the revenue field by comparing it with quantity, unit price and discount. The calculated values matched the provided revenue values, allowing for rounding."
"The dataset contains synthetic transaction dates spanning 2022–2035."
#Data validation
Revenue Validation: Revenue = Quantity × Unit Price × (1 - Discount)
=IF(ABS([@Revenue_Difference])<0.02,"Valid","Check")
