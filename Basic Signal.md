#Conttime 

In signal processing, a signal is a function that conveys information about a phenomenon. Signals can be classified into two main categories: periodic and non-periodic signals. In this atomic note, we will focus on basic non-periodic signals.

## Definition of Non-Periodic Signals

A non-[[periodic signal]], also known as an aperiodic signal, is a signal that does not repeat itself over time. Unlike periodic signals, which exhibit a regular pattern and have a [[fundamental period]], non-periodic signals have no such repeating pattern.

## Unit Impulse Function

One of the most fundamental non-periodic signals is the unit impulse function, denoted as $\delta(t)$. The unit impulse function is defined as:

$$
\delta(t) = \begin{cases} 
      0 & t \neq 0 \\
      \infty & t = 0 
   \end{cases}
$$

The unit impulse function has an area of unity and an infinitely high amplitude at $t = 0$. It can be thought of as an idealized mathematical representation of an instantaneous [[event]].

## Unit [[Step Function]]

Another important non-[[periodic signal]] is the unit [[step function]], denoted as $u(t)$. The unit [[step function]] is defined as:

$$
u(t) = \begin{cases} 
      0 & t < 0 \\
      1 & t \geq 0 
   \end{cases}
$$

The unit [[step function]] has a value of zero for negative values of $t$ and a value of one for positive or zero values of $t$. It represents an instantaneous change from zero to one at $t = 0$.

## [[Ramp Function]]

The [[ramp function]], denoted as $r(t)$, is another commonly encountered non-[[periodic signal]]. It is defined as:

$$
r(t) = \begin{cases} 
      0 & t < 0 \\
      t & t \geq 0 
   \end{cases}
$$

The [[ramp function]] has a linearly increasing value for $t \geq 0$ and zero value for $t < 0$. It represents a gradual increase over time.

## Exponential Function

The exponential function, denoted as $e^t$, is an essential non-[[periodic signal]]. It is defined as:

$$
e^t = \sum_{n=0}^{\infty} \frac{t^n}{n!}
$$

The exponential function grows exponentially with time. It is commonly encountered in various fields, including physics, engineering, and finance.

## Conclusion

Non-periodic signals play a crucial role in signal processing. The unit impulse function, unit [[step function]], [[ramp function]], and exponential function are some of the fundamental non-periodic signals. Understanding these basic non-periodic signals is essential for analyzing and processing more complex signals encountered in various applications.