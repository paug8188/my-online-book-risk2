# Brief Introduction on Risk

My intention to learn about data analytics comes from the interest of quantifying risk.
If we have enough sample data of a scenario, combines it with the law of probability, we can quantify the risk.
We will encounter risk on our daily basis or at work whenever we need to make a decision. 
Informed decision always need data analytics.

```{margin} When did the serious study of risk begin?
It was in 1654, when the Rennaisance era was blooming!
```

## Definition of Risk

I am quoting this from a book called {cite}`against_the_gods`

> "The word "risk" derives from the early Italian *risicare*, which means "to dare". In this sense, risk is a choice rather than a fate. The actions we dare to take, which depend on how free we are to make choices."

```{figure} https://i.gr-assets.com/images/S/compressed.photo.goodreads.com/books/1541411380l/128429.jpg
---
height: 300px
name: against-the-gods-cover
---
The Bible for Risk Managers
```

```{note}
This book is not a light reading but it is really interesting.
```

## Law of Probability

Still from the same book, {cite}`against_the_gods` {numref}`against-the-gods-cover`, I read that human beings started to quantify risk to win a gamble. It all started for a practical reason and based on human greed.
Betting is about how to win the odds. Game of chance like flipping a coin has a 50:50 odds.
So, assuming that I would like to toss the coin until I see the first tail then I would stop tossing. 
if $ \chi $ is the total number of tossing, and $ \chi = 4 $, what is the probability of getting the tail at the end when tossing the coin 4 times?

```{figure} https://cdn.pixabay.com/photo/2020/12/11/09/05/coin-flipping-5822271_1280.png
---
height: 300px
name: coin-flipping
---
Game of Chance
```

Here is the general formula:

```{math}
:label: prob_eq_label
P(A \cap B) = P(A)P(B)
```
Just remember:

```
probability = P
outcome of the experiment = \chi
event = H or T
```

```
P(4) = P(HHHT)
```


So if we apply to the question using {eq}`prob_eq_label`, here is the implementation:

```{math}
:label: coin_eq_label
P(HHHT) = P(H)P(H)P(H)P(T)
        = \frac{1}{2}*\frac{1}{2}*\frac{1}{2}*\frac{1}{2}
        = \frac{1}{16}
```

In conclusion, using {eq}`coin_eq_label`, the probability of getting the tail {numref}`coin-flipping` after 4 tosses is  $ \frac{1}{16} $



```{warning}
Please don't be a gambler after this!
```
