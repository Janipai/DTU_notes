Output k <- K forstås som:
K is a finite set to mean that x is sampled from the uniform distribution K

$\{0, 1\}^\lambda$ hvor lambda er lambda-bit binary string and 0,1 is denoted the set of all binary strings. 
### Exercise 1
k,m,c is sampled according to keyspace K, M, C

$$
K = M = C = \{0,1\}^\lambda
$$


$KeyGen():$
$$Output\: k \leftarrow K $$
$Enc(k,m \in M):$
$$
Output\: k\&m
$$

you miss information when you use the and operator
$$
c = Enc(k,m) = k_i \& m_i 
$$
Example
$$
k_i= 0
$$
$$
m_i= 1
$$
$$
c_i = k_i\&m_i = 0\&1 = 0
$$

$Dec(k,c \in C):$
$$
Output\: k\&c
$$
$$
m' = k\&c
$$
$$
m_i' = k_i\&c_i = 0\&0 = 0
$$
this m is not the same as the encrypted m
$$m_i'\neq m_i$$

### Exercise 2
#### 1.
k,m,c is sampled according to keyspace K, M, C
$$
K = M = C = \{0,1\}^\lambda
$$
$KeyGen():$
$$Output\: \pi \leftarrow S $$
$Enc(\pi,m \in M):$
$$
Output\: \pi(m)
$$
The cipher text is defined to be
$$
c=\pi(m)
$$$Dec(\pi,c \in C):$
$$
Output\: \pi^{-1}(c)
$$
The plain text is the inverse of the $Enc(\pi,m)$
$$
\pi^{-1}(c)=\pi^{-1}(\pi(m))=m
$$
#### 2.
The encryption algorithm takes two arguments and output the encrypted version of the argument. If we set these two arguments to be different bits that are one bit long, then the output will tell which argument it is operating on. These two bits would be 0 and 1. This is due to permuntation (alle typer af omrokering). 

```
FnA(a,b)
	return a
```
