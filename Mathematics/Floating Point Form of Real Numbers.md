---
date: 2022-08-16
type: 🧠
tags:
  - MAC/3/MN1
---

**Topics:** [[Numerical Analysis]] - [[Rounding Error]] - [[Normalised Form of Real Numbers]]

---

The floating point form of a number in its [[Normalised Form of Real Numbers|normalised form]] can be obtained by terminating the fractional part of the number at $k$ digits. There are two ways to do this:

- **Truncate:** the digits of the number up to the position that the [[Word (computer archihtecture)|word]] size allows (i.e. $k$)
- **Round:**
	- If $d^{k+1} \geq 5$, we add $1$ to $d^k$, "_rounding up_"
	- If $d^{k+1} < 5$, we ignore the digits from $k+1$ onward, "_rounding down_"

$k$ is dependant on the size of the [[Word (computer archihtecture)|computer word]].

# Bit Assignation and Range

Floating point numbers use specific bits of the [[Word (computer archihtecture)|computer word]] for specific purposes. Normally, there's 1 bit dedicated to the sign, several bits for the [[Exponent|exponent]], and some more for the [[Mantissa|mantissa]] (the fractional part of the number).

## Range and Exponent

The size of the word defines the range of the exponent of the floating point number:

| **Total digits** | **Range of the exponent**         | **Exponent**            |
| -------------------- | ----------------------------- | ------------------- |
| $N = p + q + 1$      | $-(2^{p-1} - 1)$ to $2^{p-1}$ | $c - (2^{p-1} - 1)$ |

…where:

- $p$: number of digits for the exponent
- $q$: number of digits for the mantissa
- $c$: decimal form of the number in the exponent part of the word

> [!warning]- Mantissa Bits
>
> Please note that the mantissa section of the word must **always** have $1$ in its first position (left to right). The mantissa section **cannot** be $0$ in total.

# Final Number

The final number as represented on the computer is given by:

$$
(-1)^{s} B^{e} (1 + f)
$$
…where:

- $s$: the bit corresponding to the sign
- $e$: the exponent (i.e. $c - (2^{p-1} - 1)$)
- $f$: the decimal number in the mantissa section
- $B$: the base for the numbering system

> [!example]-
>
> For instance, take the following number as represented in bits:
>
> | $s$ | Exponent  | Mantissa            |
> | --- | --------- | ------------------- |
> | 1   | 1 0 0 1 1 | 1 0 0 1 0 1 0 0 0 0 |
>
> In this case, we have that:
>
> - $s = 1$
> - $e = 19 - 15 = 4$
> - $f = 0.1001010000_{2} = 0.578125_{10}$
>
> Thus, the number is:
>
> $$
> (-1)^{1} 2^{4} (1 + 0.578125)
> $$
>
> $$
> =-16(1.578125) = -25.25
> $$
