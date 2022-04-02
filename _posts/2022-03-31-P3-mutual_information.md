---
title: "Mutual Information vs Correlation Coefficient"
---

---
## Mutual Information Definitions:

> "The mutual information (MI) of 2 random variables is a measure of the mutual dependence between 2 variables." - Wikipedia

> "The Mutual Information between 2 random variables is the amount of information that one gains about a random variable by observing the value of the other." - Layman's term

![image](https://user-images.githubusercontent.com/79191009/161368320-fe7dc1f3-01c1-48c3-996e-fe1f49aaa1e9.png)

![image](https://user-images.githubusercontent.com/79191009/161368343-bf438686-b63d-4a4e-b3a2-11a7c37da605.png)




## Correlation Coefficient Definitions:

> "Pearson's correlation coefficient is a measure of linear correlation between two sets of data." - Wikipedia

![image](https://user-images.githubusercontent.com/79191009/161366454-3fa5fec6-0b0b-457d-a4a2-6f3e525ef2af.png)

- As shown in [Anscombe's quartet](https://en.wikipedia.org/wiki/Anscombe%27s_quartet) graphical check is required when using correlation coefficient
- Common Correlation range:
    - Small: 0.10 to 0.29
    - Medium: 0.30 to 0.49
    - Large: 0.50 to 0.10

---

## Comparison with Correlation Coefficient

| Metric | MI | Correlation |
|--------|----|-------------|
| Intuition | Measure of "knowledge" or "information" gain from knowing another variable. | Quantitative measure of linear relationship between 2 variables |
| Value Range | 0 to 1 | -1 to 1 |
| Value Interpretation | Higher MI, higher importance | Closer to either extreme, stronger linear relationship |

---
References
1. [Mutual Information](https://en.wikipedia.org/wiki/Mutual_information)
2. [Correlation and Mutual Information](https://eng.libretexts.org/Bookshelves/Industrial_and_Systems_Engineering/Book%3A_Chemical_Process_Dynamics_and_Controls_(Woolf)/13%3A_Statistics_and_Probability_Background/13.13%3A_Correlation_and_Mutual_Information#:~:text=Correlation%20analysis%20provides%20a%20quantitative,the%20value%20of%20another%20variable.)
3. [Correlation vs Mutual Information](http://www.mathemafrica.org/?p=16127)
