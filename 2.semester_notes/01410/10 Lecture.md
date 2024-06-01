True or false
DLOG is harder than DDH, and DHH is harder than CDH

Dicrete Log prblem (DLOG)
given(p, g, g^a) -> find a

Computational Diffie Hellman prblem (CDH)
given(p, g, g^a, g^b) -> find g^(ab)

Decisional Diffie Hellman problem (DDH)
Given either
(p,g,g^a,g^b,g^(ab))
or
(p,g,g^a,g^b,g^c)

the first part is true and the second is false??

A key agreement protocol is considered secure if the key output by the  
participants is indistinguishable from an independent uniformly  
random key, given the transcript of protocol messages.  

is true

Diffie hellman key aggrement protocol is NOT secure against active attacks
_____
The concept of groups:
a groupe is a set S and a binary operation(a binary operation is when taking two inputs and output one output) $\circ : S \times S -> S$

Associativity
$\forall a,b,c \in S : (a\circ b)\circ c=a\circ (b\circ c)$

Identity
$\exists e \in S \forall a \in S$
$a\circ e=e\circ a=a$

A group here $a\circ b = b\circ a$ for all $a, b \in S$
is called commutative (Abelian)

the order of the element (ex $g⁰=e,g¹=g,g²,g³..$)