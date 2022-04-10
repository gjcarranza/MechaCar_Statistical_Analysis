# MechaCar Statistical Analysis

---

# Linear Regression to Predict MPG

* Pr(>|t|) column indicates non-random amount of variance to the mpg values in the dataset
* Statistical significance of the p-value is less than 0.05% (i.e. the p-value is 5.35e-11), therefore not zero
* Looking at the multiple R-squared value of 0.7149 (valued at 71.49%), it is fair to say that the linear model can predict the mpg of MechaCar prototypes fairly accurately.

![summary_MechaCar_mpg](https://user-images.githubusercontent.com/92961267/162628132-e0f599ad-9d1e-4b93-8b76-dbcd4a49fb40.png)

---

# Summary Statistics on Suspension Coils

![total_summary](https://user-images.githubusercontent.com/92961267/162628140-7b3051b6-69eb-46c5-991f-5f66f7ab692c.png)

* Initially looking at the total summary variance value, it does not exceed more than 100 pounds per square inch, hence initially meeting design specification for all manufacturing lots.

![lot_summary](https://user-images.githubusercontent.com/92961267/162628150-95b112ae-ddcd-4840-bfd8-9301291c84d9.png)

* Upon closer inspection only lots 1 and 2 variance values are deemed to meet the design specification as lot 3 exceeds the specification meaning that there are significantly large outliers in lot 3

---

# T-test for Suspension Coils

![t_test_Suspension_Coil](https://user-images.githubusercontent.com/92961267/162628168-a7897891-36c4-4f98-bfab-f2fec168d4bb.png)

* Further analysis of the total t-test summary for Suspension Coil, the p-value (0.06028) is great than 0.05% and can be determined as there is no statistical significance or evidence exclaiming that the PSI for the total manufacturing lot deviates from the population mean of 1500 pounds per square inch.

![t_test_lots_1_to_3](https://user-images.githubusercontent.com/92961267/162628172-84f4d5ce-84d1-4882-b03c-600c430d77ac.png)

* Upon further analysis when viewing the p-values for the lots individually, a similar a conclusion can be given to that of the total manufacturing lot for lots 1 and 2. Lot 3 deviates from this trend, ergo is statistically significant.

---

# Design Study to Compare to Competition

In order to compare this linear regression model to other comptetitors, it is best to obtain datasets of other competitors and compose a similar model. There is a possibility that other competitors' models may provide a fair accuracy level with respect to predicting mpg prototypes. The exception that there is a possibility that the lot(s) of cars of competitors may go through a more selective, and rigorous regime to evade production troubles. The possibility of comparing the prototype to similar models can produce a unique hypothesis: based on the performance of the MechaCar, its value is fair. The opposite can also be true, but will not be conclusive upon further analysis. A suggestion is to use chi-squared testing to see if the frequencies are within reason of what may be expected and ANOVA testing to do multiple comparisons of signifcant statistical values to compare to other competitors.
