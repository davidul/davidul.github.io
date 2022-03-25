+++
author = "David Ulicny"
title = "Digital root"
date = "2022-03-25"
description = "Digital root"
tags = [
    "digital root",
    "numbers",
]
categories = [
    "digital root",
]
+++

# Digital root

Digital root or digital sum of non-negative integer
is the sum of digits in the number. The result is single digit number, for example

$$
256 = 2 + 5 + 6 = 13 = 1 + 3 = 4
$$

Properties of digital root:
* if we multiply any number by 9, the digital root will be always 9
* adding 9 to a number does not change the digital root
* if we divide any number by 9 the remainder is the digital root

$$
9 \equiv 0(\mod 9)
$$

It is also true that for any multiple of 9

$$
9x \equiv 0 (\mod 9)
$$

Calculate digital root

```
if(n == 0) return 0;
if(n % 9 == 0) return 9;
return n % 9;
```

## Application of digital root