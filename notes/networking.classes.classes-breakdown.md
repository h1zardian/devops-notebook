---
id: h9b7lp196dwynsepmw0anfa
title: Classes Breakdown
desc: ''
updated: 1663687913275
created: 1662656428510
---

- IP address for `IPv4` is of 32 bits. So it's **4** sets of **8 bits** or 1 byte.

- It is represented in the decimal format.

- So converting any sets of octet of IPv4 in binary will give us:
 
> $x \dotsi x \dotsi x \dotsi x$  
> $8$  
> $2^7\space\space\space$  $\space\space2^6\space\space$  $\space\space2^5\space\space$  $\space\space2^4\space\space\space$  $\space\space\space2^3\space\space$  $\space\space2^2\space\space$  $\space\space2^1\space\space$  $\space\space2^0$  
>$128\space$ $\space64\space\space$ $\space32\space\space$ $\space\space16\space\space$ $\space\space\space\space8\space\space$ $\space\space\space\space4\space\space$ $\space\space\space2\space\space\space$ $\space\space\space\space1$

><pre>
                                                 class
0    0    0    0    0    0    0    0  =  1 -126    A
1    0    0    0    0    0    0    0  = 128-191    B
1    1    0    0    0    0    0    0  = 192-223    C
1    1    1    0    0    0    0    0  = 224-239    D
1    1    1    1    0    0    0    0  = 240-255    E
</pre>
