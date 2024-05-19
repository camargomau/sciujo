---
date: 2024-05-18
type: 🧠
tags:
  - MAC/6/PE
---

**Topics:** [[Queuing Model]] - [[Birth-Death Markov Process]]

---

_**(definition)**_

An **$M/M/S$ queue** is a [[Queuing Model|queuing model]] where:

- The arrivals are determined by a [[Homogeneous Poisson Process|Poisson process]] (i.e. they follow a [[Poisson Distribution|Poisson distribution]])
- The service times distribute [[Exponential Distribution|exponentially]]
- There are $S$ servers

_**(observation)**_

Notice that this is basically a [[Birth-Death Markov Process|birth-death Markov process]], since their arrivals also follow a Poisson process and the time between deaths also distributes exponentially.

# Arrival and Service Rates

> [!tip]- $\lambda$ and $\mu$
> In a queuing model, $\lambda_{n}$ is the [[Expected Value|expected]] rate of arrivals per unit of time when there are $n$ clients in the system, while $\mu_{n}$ stands for the expected rate at which clients are being serviced per unit of time when there are $n$ clients in the system. 

_**(theorem)**_

A $M/M/S$ queue has the following rates:

- If $S=1$, then:
	- $\lambda_{n} = \lambda$ for $n = 0, 1, 2, \dots$
	- $\mu_{n} = \mu$ for $n = 1, 2, 3 \dots$
- If $S>1$, then:
	- $\lambda_{n} = \lambda$ for $n = 0, 1, 2, \dots$
	- $\mu_{n} = n\mu$ for $n = 1, 2, 3 \dots$
		- Alternatively, $\mu_{n} = S\mu$ for $n = S, S+1, S+2, \dots$

We consider an $M/M/S$ queue stable when its utilisation factor $\rho = \frac{\lambda}{S\mu}$ satisfies $\rho<1$ (i.e. $\lambda<\mu$).

# Performance Measures for $M/M/1$

_**(theorem)**_

When $S = 1$, the model is $M/M/1$ and its [[Performance Measures for a Queuing Theory Model|performance measures]] are:

- $\rho=\frac{\lambda}{\mu}$ (utilisation factor)
- $C_{n} = \left( \frac{\lambda}{\mu} \right)^{2} = \rho^n$ for $n = 0, 1, 2, \dots$
- $P_{n} = \rho^n(1-\rho)$ for $n = 0, 1, 2, \dots$ (the probability of having $n$ clients in the system)
- $L = \frac{\lambda}{\mu-\lambda}$ (the [[Expected Value|expected]] amount of clients in the system)
- $L_{q} = \rho L =\frac{\lambda^{2}}{\mu(\mu -\lambda)}$ (the expected amount of clients _in the queue_)
- $W = \frac{1}{\mu-\lambda}$ (the expected wait time in the system)
- $W_{q} = \rho W = \frac{\lambda}{\mu(\mu-\lambda)}$ (the expected wait time _in the queue_)

Do note that this assumes that the system is stable (i.e. $\rho < 1$).

