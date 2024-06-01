Exercise 1.1
Find the missing 3DES.Dec

$3DES.Dec(k,c)$
$$
DES.Dec(k3,DES.Enc(k2,DES.Dec(k1,c)))
$$
Exercise 1.2
a)
It takes 1 ns to calculate 1 key and the key is $2^{56}$ long (7.2057594e+16) and we know that there is $8.64\cdot 10³$ ns on one day

$$
2^{56}/(8.64 \cdot 10^{13})/365=2.28
$$
So it takes 2,28 years to calculate one key

Exercise 1.2
b)
We parallelize the process and distribute the calculation out to each machines.

$$
2^{56}/(8.64 \cdot 10^{13})/1024=0.81
$$
it takes 0.81 day to brute-force the key 

Exercise 1.2
c)

we do the same, just with 13.8 billion years
$$
2^{56\cdot3}/(8.64 \cdot 10^{13})/365/(13.8\cdot10^{9})/1024=8.40e+20
$$
It takes 8,40e+20 years of the universe 

Exercise 2
a)
Lookup function for real and for rand

real
Output
$Lookup(x\in{0,1}^{in})$
$y\leftarrow \: G(k,x)$
$Output \: y$

rand
is the same from slide 27

b)
Output
$Lookup(x\in{0,1}^{in})$
$y\leftarrow \: F(k,x)\bigoplus r$
$Output \: y$

c)
