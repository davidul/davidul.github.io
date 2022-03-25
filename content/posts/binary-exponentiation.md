+++
author = "David Ulicny"
title = "Binary exponentiation"
date = "2022-03-25"
description = "Binary exponentiation"
tags = [
    "binary",
]
categories = [
    "binary",
]
+++


# Exponents rules

$$
a^{m} \cdot a^{n} = a^{m+n}
$$


$$
\frac{a^{m}}{a^{n}} = a^{m-n}
$$

$$
(a^{m})^{n} = a^{m \cdot n}
$$


# Binary exponentiation

Exponentiation means to multiply `a` b-times. 

$$
a \cdot a \cdot a = a^{b}
$$

Multiplying each term b-times will give O(b) complexity.


Demonstrate binary exponentiation on 

$$
2^{10}
$$

Lets write 10 in binary  `1010`. The corresponding bits will be used

$$
2^{10} = 2^{8} + 2^{2}
$$

$$
\begin{align}
2^{1} = 2 \newline
2^{2} = (2^{1})^{2} = 2^{2} = 4 \newline
2^{4} = (2^{2})^{2} = 4^{2} = 16 \newline
2^{8} = (2^{4})^{2} = 16^{2} = 256 \newline
\end{align}
$$

## Modular binary exponentiation