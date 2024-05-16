
Forward probability is a concept in probability theory that describes the likelihood of an event occurring in the future, given the current information available. It is often used in financial mathematics to model the uncertainty of future events and make predictions about their likelihood.

## Definition

The forward probability $P(A_t)$ of an event $A$ occurring at time $t$ is defined as the conditional probability of $A$ given all the information available up to time $t$. Mathematically, it can be expressed as:

$$P(A_t) = P(A \mid \mathcal{F}_t)$$

where $\mathcal{F}_t$ represents the information available at time $t$. This information can include past events, market data, and other relevant factors that may affect the occurrence of event $A$.

## Key Theorems

### Bayes' Theorem
([[Bayesian]])
Bayes' theorem is a fundamental result in probability theory that relates conditional probabilities. It states that for two events $A$ and $B$, the following holds:

$$P(A \mid B) = \frac{P(B \mid A) P(A)}{P(B)}$$

where $P(B)$ is known as the prior probability of event $B$, and $P(A)$ is known as the prior probability of event $A$. This theorem plays a crucial role in calculating forward probabilities by incorporating new information into existing probabilities.

### Markov Property

The Markov property states that for a stochastic process, future events are independent of past events given the present state. In other words, knowing the current state is sufficient to predict future states. This property is essential in modeling forward probabilities as it simplifies calculations by reducing dependence on past events.

## Examples (wrong math)

Let's consider an example where we want to calculate the forward probability of a stock price increasing by 10% within one year. We have the following information available:

- The current stock price is $100.
- The stock has a 50% chance of increasing by 10% in the next year.
- The stock has a 50% chance of decreasing by 5% in the next year.

Using Bayes' theorem, we can calculate the forward probability as follows:

$$P(\text{Increase}) = \frac{P(\text{Increase} \mid \text{Up}) P(\text{Up})}{P(\text{Increase} \mid \text{Up}) P(\text{Up}) + P(\text{Increase} \mid \text{Down}) P(\text{Down})}$$

where $P(\text{Up}) = 0.5$ and $P(\text{Down}) = 0.5$. Now, we need to calculate the conditional probabilities $P(\text{Increase} \mid \text{Up})$ and $P(\text{Increase} \mid \text{Down})$. Using the Markov property, we can assume that these probabilities are independent of past events and only depend on the current state.

Therefore, $P(\text{Increase} \mid \text{Up}) = 0.5$ and $P(\text{Increase} \mid \text{Down}) = 0$, since if the stock price increases by 10%, it cannot simultaneously decrease by 5%.

Substituting these values into our equation, we get:

$$P(\mathrm{\ Increase\ }) =\frac{(0.5)(0.5)}{(0.5)(0.5) + (0)(0.5)} =\frac{(1/4)}{(1/4)}=1$$

This means that our forward probability of the stock price increasing by 10% within one year is 100%.

## Conclusion

Forward probability is a powerful tool in predicting the likelihood of future events. It allows us to incorporate new information into existing probabilities and make more accurate predictions. By understanding key theorems such as Bayes' theorem and the Markov property, we can effectively calculate forward probabilities and make informed decisions in various fields, including finance and economics.