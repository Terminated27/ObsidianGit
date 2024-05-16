#stats 

Bayesian statistics is a branch of statistics that uses probability theory to make inferences about unknown quantities or parameters. It is based on the Bayes' theorem, which provides a way to update our beliefs about a particular [[event]] or hypothesis as we gather more evidence or data.

## Bayes' Theorem

Bayes' theorem is the fundamental concept behind Bayesian statistics. It states that the posterior probability of an [[event]] A given evidence B is equal to the prior probability of A multiplied by the likelihood of B given A, divided by the marginal likelihood of B.

$$P(A|B) = \frac{P(B|A)P(A)}{P(B)}$$

where:

- $P(A|B)$: posterior probability of A given B
- $P(B|A)$: likelihood of B given A
- $P(A)$: prior probability of A
- $P(B)$: marginal likelihood of B

Bayes' theorem allows us to update our beliefs about an [[event]] or hypothesis as we gather more evidence. This makes it a powerful tool for making predictions and decisions based on uncertain information.

## Bayesian Inference

Bayesian inference refers to the process of using Bayes' theorem to update our beliefs about an [[event]] or hypothesis as we gather more evidence. It involves two main steps:

1. **Prior belief**: We start with an initial belief about the [[event]] or hypothesis, represented by the prior probability $P(A)$.
2. **Update with evidence**: As we gather more evidence, we use Bayes' theorem to update our belief and calculate the posterior probability $P(A|B)$.

This process can be repeated multiple times as new evidence becomes available, allowing us to continuously refine our beliefs and make better predictions.

## Example: Coin Toss

Let's consider a simple example where we want to determine whether a coin is fair (equal chance of landing heads or tails) or biased towards heads. Our prior belief is that the coin is fair, represented by $P(A) = 0.5$. We then toss the coin 10 times and get 7 heads and 3 tails. We can use Bayes' theorem to update our belief:

$$P(A|B) = \frac{P(B|A)P(A)}{P(B)} = \frac{0.5^7 \times 0.5^3}{\binom{10}{7}0.5^{10}} = \frac{\binom{10}{7}}{2^{10}} \approx 0.12$$

The posterior probability of the coin being fair given the evidence is only 12%. This suggests that the coin may be biased towards heads.

## Bayesian Hypothesis Testing

Bayesian hypothesis testing is a method for comparing two competing hypotheses based on their posterior probabilities. It involves calculating the Bayes factor, which is the ratio of the posterior probabilities of the two hypotheses:

$$B_{01} = \frac{P(H_0|D)}{P(H_1|D)} = \frac{\int P(D|\theta,H_0)P(\theta|H_0)d\theta}{\int P(D|\theta,H_1)P(\theta|H_1)d\theta}$$

where:

- $H_0$: null hypothesis
- $H_1$: alternative hypothesis
- $D$: observed data
- $\theta$: parameters of the model

If $B_{01} > 1$, then there is more evidence in favor of $H_0$ compared to $H_1$. If $B_{01} < 1$, then there is more evidence in favor of $H_1$.

## example
$$
\begin{numcases}{f_{X,Y}(x,y) = }
8xy, 0\le x \le 1, x \le y \le 1\\
0, else
\end{numcases}
$$
estimators of X given Y
$$
f_{X|Y}(x|y)=\frac{f_{X,Y}(x,y)}{f_Y(y)}
$$
$$
\begin{cases}
\frac{2x}{y^2},0\le y \le 1, 0\le x \le y\\
0, else
\end{cases}
$$
given that $y=\frac{1}{2}$ what is a good guess for $X$
$$
\begin{numcases}{f_{X|Y}(x|y) = }
8x, 0 \le x \le 1\\
0, else
\end{numcases}
$$

## Conclusion

Bayesian statistics provides a powerful framework for making inferences and predictions based on uncertain information. It allows us to update our beliefs as we gather more evidence and make better decisions based on this updated knowledge. By using Bayes' theorem and Bayesian inference, we can tackle complex problems and make accurate predictions in various fields such as medicine, finance, and engineering.
