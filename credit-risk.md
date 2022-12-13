# Credit Risk

One of the risk that is relevant to our day to day life is credit risk. 

:::{admonition} what is credit risk?
:class: tip, dropdown
Credit risk is the possibility that a borrower or counterparty would fail to meet its debt obligations.
:::

```{figure} https://www.piranirisk.com/hs-fs/hubfs/20_riesgo_crediticio.jpg?width=1188&name=20_riesgo_crediticio.jpg
---
height: 300px
name: credit-risk
---
Credit Risk 
```

There are a lot of sub-categories of credit risk but for this purpose, I will not go further into detail.
Something relevant to us pertaining to credit risk is a credit rating.
This is a report to evaluate if someone or an entity is credit-worthy for financial institutions.

```{margin} How do you know your credit rating?
Equifax and TransUnion are two big credit bureaus in Canada. You can get your credit report for free!
```

```{figure} https://icash.ca/images/learn/major-credit-bureaus.jpg
---
height: 300px
name: credit-bureau
---
Equifax and TransUnion
```

```{note}
Whenever you apply for financing, the financial institution will ask to grant access to your credit report.
```

For ilustration, TransUnion generated a credit score for individuals ranging between 300 to 900.
There are ranges to evaluate your creditworthiness as follows:

```
Excellent = 833 <= $\chi$ <= 900
Very Good = 790 <= $\chi$ <= 832
Good = 743 <= $\chi$ <= 789 
Fair = 693 <= $\chi$ <= 742 
Poor = 300 <= $\chi$ <= 692
```

Where $\chi$ is your score

To code this, we can use loc function:

```python
credit_score_df.loc[credit_score_df['score'] >= 833 and credit_score_df['score'] <= 900, 'Creditworthiness' = 'Excellent']
so on
```


```{math}
:label: credit_score
\chi = \omega_1 \cdot \ipsilon_1 + \omega_2 \cdot \ipsilon_2 + ... + \omega_N \cdot \ipsilon_N
```

How is the credit score calculated?
Typically it is calculated using different metrics with their relative weights just like the formula ilustrated on {eq}`credit_score`



