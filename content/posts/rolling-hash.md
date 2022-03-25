+++
author = "David Ulicny"
title = "Rolling Hash"
date = "2022-03-11"
description = "About rolling hash"
tags = [
    "algorithm",
    "rolling hash",
]
categories = [
    "algorithms",
    "rolling hash",
]
series = ["Basic"]
draft = true
+++

# Rolling hash

$$
hash(s) = s[0] + s[1] \cdot p + s[2] \cdot p^{2} + ... + s[n - 1] \cdot p^{n-1} \mod m
$$

In short 

$$
\displaystyle\sum_{i=0}^{n-1} s[i] \cdot p^i \mod m
$$