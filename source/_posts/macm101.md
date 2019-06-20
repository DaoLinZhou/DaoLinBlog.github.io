---
title: HelloWorld
date: 2013-12-24 23:29:53
tags:
- Foo
- Bar
- Baz
header_image: /intro/post-bg.jpg
typora-copy-images-to: asserts
---



# MACM101

## 特殊符号

```
¬ ∀ ∃ ∈ ∉ ⊆ △ ∩
```



## ---Counting---

![](assets/counting.png)

**Ex.1-1**

Choose one group activity how many choice?

4 + 2 = 6

4 movies 2 board games

**Ex.1-2**

Choose one movie then play a board game, how many choices?

4 * 2 = 8



### The Rule of Sum:

• If a first task can be performed in m ways

and a second task can be performed in n

ways, and the two tasks are mutually

exclusive (cannot be performed

simultaneously), then performing either

task can be accomplished in any one of m+n ways (Ex. 1-3)



### The Rule of Product:

• If a task can be broken down into the first

and second stages, and if there are m

possible outcomes for the first stage and n

possible outcomes for the second stage,

then the whole task can be accomplished 

in m·n ways (Ex. 1-4) 



Ex.1.7

How many different ways are there to re-arrange the
letters in the word “ART”? 



3! = 3 * 2 * 1 = 6



Ex.1.8

There are 25 students in this class, the top five
students will receive an A, how many such
arrangements are there? 



​	25 * 24 * 23 * 22 * 21

=	25! / (25-5)!



### P(n, r)

If there are n distinct objects, and r is an integer
(1 ≤ r ≤ n), then the number of permutations of size
r of these n objects is defined as: 
$$
P(n, r) = n(n-1)(n-1)...(n-r+1)
		= n!/(n-r)!
$$




If there are n objects with:
- n1 indistinguishable objects of type 1,

- n2 indistinguishable objects of type 2,
  :
  :

- nr indistinguishable objects of type r
  and n1 + n2 + ... + nr = n, then there are 
  $$
  n! / n1!n2!...nr!
  $$
  



![](assets/ur.jpg)







how many ways from (1, 1) to (6, 4)

up -> u

right -> r

so it can change to find how many ways to connect "uuurrrrr".

8! / (3! * 5!)



Ex.1-15

For example in (Ex.1-8), the 5 students who
receive an A in this course will not care what order
they are in (as long as they receive an A)  25  students.



So a-b-c-d-e & b-d-e-c-a  are same

25! / (20! * 5!)



### C(n, r)

Given n distinct objects, a combination (or
selection) of r objects (0 ≤ r ≤ n) without order
corresponds to r! permutations of size r from the n
objects.
•The number of combinations C(n,r) of size r from
the n objects is 

![](assets/cr.png)



Ex.1-18

Anagrams of the word “TALLAHASSEE”
such that no two ʻAʼs are adjacent 



1) pick out A

T L L H S S E E

there are 8!/(2! * 2! * 2!) ways to sort them.



2) then insert A in to each gap

8 letters so there are 9 gaps.

therefore choose 3 from 9 is C(9, 3)

Answer is :	8! * C(9, 3) /(2! * 2! * 2!) 



Ex. 

9 women ,6 men sit around circle.

no men sit in together



1) 9 w sit in circle = 9!/9

2) 9 empty choose 6 for men = C(9, 6)

3) 6 different men have 6! choices

 * women are fixed.

   so it is no longer be a circle.

   therefore men have 6! choices but not 5! choices.



### Combination - Summation Notation

Given a list of terms am, am+1, am+2, ... , am+n, where m
and n are integers (n≥0), a summation can be written
in Sigma (∑) notation as: 



![](assets/20190507202814.png)

​				

### Combination - Binomial Theorem 

If x and y are variables and n is a positive integer,

![](assets/20190507203043.png)





why?

for example :

(x+y)^3 = (x1+y) (x2+y) (x3+y)

if we looking for the const before x^2 * y

that means we choose 2 of x form x1, x2 ,x3

that is C(3, 2)



Let n be an integer (n>0), then

![](assets/20190507203431.png)



why?

(1+1)^n = 2^n

also it fits (x+y)^n

same reason

(1-1)^n = 0^n



### Combinations - Multinomial Theorem

![](assets/x1x2x3.png)

(x1+x2+x3)^9 

C x1^3 * x2^4 * x3^2

C = 9! / (3! * 4! *2!)





### Combinations - with repetition

**EX.**

7 students in the restaurant. There are 4 options for them a, b, c, d.

How many different purchases are possible(from the view point of the restaurant)



from the view point of the restaurant, so 7 student are the same, restaurant don't care who wants what



possible ways:

aaa bb c d	->	### | ## | # | #

aaaaaaa	    ->	####### | | |

abbcccc	     ->	# | ## | #### |

3 dividers, 7 students

7+4-1 = 10 spaces

choose 7 for the student the rest are for dividers.

answer is (10 choose 7)



![](assets/repetition.png)

It is also like put 7 balls into 4 boxes(a, b, c, d)

answer is same.



**Ex.2**

x1 + x2 + x3 + x4 = 8;

x1-x4 are all >= 0

how many ways?

It's just like put 8 balls in to 4 bags, 8+4-1 = 11

answer is (11 chooses 8)



**Ex.3**

x1 + x2 + x3 + x4 = 32

xi >= -2

1. get 2 from every box (x), 32 + 2 + 2 +2 = 40
2. put 40 back to each box(x)

40+4-1 = 43

answer is (43 choose 40)





## ---Logic---

### Logical Connectives

Statement (propositions) are declarative sentences that are either true or false.

Truth values of proposition can be true (T or 1) or false (F or 0)

#### Logic operations:

- Not (negation)
- AND(conjunction)
- OR (disjunction)
- XOR(exclusive OR)
- Implication
- Biconditional



##### Negation (not)

" ¬ " mean negation

p  	1	0

¬p	0	1

when p is true ¬p is false



##### Conjunction (and)

" ^ " means conjunction

p    	0	0	1	1

q    	0	1	0	1

p^q	0	0	0	1

the proposition is true when **both** p and q are true.



##### Disjunction (or)

" v " means disjunction

p		0	1	0	1

q		0	0	1	1

p v q	  0	1	1	1

the proposition is true when **at least** one of p and q is true.



##### Exclusive OR (Xor)

" ⊻ " means Exclusive OR

p		0	1	0	1

q		0	0	1	1

p ⊻ q	  0	1	1	0

the proposition is true when **only** one of p and q is true.



##### Implication	->

p      	0	0	1	1

q      	0	1	0	1

p->q	1	1	0	1



p is called the hypothesis, antecedent or premise

q is called the conclusion or consequence

p-> q called p is sufficient for q

​		or q is necessary for p



For example, If I got A on the course I will buy a laptop.

p	got A

q	buy a laptop

I didn't say I won't buy one if I didn't got A, Therefore, if I didn't get A. It is ok to buy one or not buy one.

But if I got A, I must buy it. If I got A and I didn't buy it, then the proposition is false.



(p1 ^ p2 ^ p3 ... pn) -> r

if any p is false then the answer is true.

only all p are true and r is false the answer is false.





##### Biconditional	<->

p if and only if q

p <-> q precisely when p->q is true and q->p is true

p		0	0	1	1

q		0	1	0	1

p<->q	1	0	0	1



p <-> q	=>	(p->q) ^ (q->p)

​		    =>	¬ (p ⊻ q)



#### tautology and contradictions

if a proposition is always true then it is tautology (T)

if a proposition is always false then it is contradiction(F)



p		1	0

¬p      	0	1

p V¬p	1	1

p^¬p 	0	0





#### tabular proofs

p : s->r	q : ¬s V r

p <=> q 	means p and q are logically equal



p	 	0	0	1	1

q	 	0	1	0	1

p->q	   1	1	0	1

¬p V q	1	1	0	1



p->q	  <=>	¬p V q

(p->q)	<->	(¬p V q)

those two are tautology, because

T <-> T 	T

T <-> F	 F

F <-> T	 F

F <-> F	 T



![](assets/algebraicproofs.png)



Ex1.

proof (x V ¬y) ^ y <=> x ^ y

​		(x V ¬y) ^ y

<=>	(x^y) V (¬y ^ y)

because ¬y ^ y is always false

so

<=>	(x^y) V false

<=>	x^y



Ex2.

p->False <=> ¬p V False <=> ¬p



Ex3. 

​	(p v q v r) ^ (p v t v ¬q) ^ (p v ¬t v r)

because p^(q v r) <=> (p^q) V (p^r)

so take p out

<=> 	p V [ (q v r) ^ (t v ¬q) ^ (¬t v r) ]

<=>	 p V [ (q v r) ^ (¬t v r) ^ (t v ¬q) ]

<=>	 p V [ (r V (q  ^ ¬t))  ^ (t v ¬q) ]

let q ^ ¬t equal to H

then ¬q v t is  ¬H

so 

<=>p V [(r V H) ^  ¬H]

<=>p V [(r ^  ¬H) V (H ^  ¬H)]

<=>p V [(r ^  ¬H) V False]

<=>p V (r ^  ¬H)

<=>p V (r ^  (¬q v t))





### Rules of Inference

Given the implication p → q, the following
implications are defined:

- The **converse** : q -> p
- The **inverse**: ¬p -> ¬q
- The **contrapositive** : ¬q -> ¬p	<=>	p -> q 



![1559078935688](assets/1559078935688.png)

Proof:

Modus Ponens (law of detachment)

```
p	// fomular above the line  we assume is true
p->q
------
q
```

True table

p		1	1	0	0

q		1	0	1	0

p -> q	1	0	1	1



we only focuse on p and p->q are true.

so q is true.



Example: 

```
proof :

1.		p->q
2.		q->(r ^ s)
3.		¬r v (¬t v u)
4.		p ^ t
		--------
		u

(1)(2): p->(r ^ s)	(5)
(4):	p			(6)
(5)(6)	(r ^ s)		(7)
(7)		r			(8)
(3)		¬r v (t->u)	(9)
(9)		r->(t->u)	(10)
(8)(10)	t->u		(11)
(4)		t			(12)
(11)(12)	u		

```



## --- Quantifiers ---

### Universal Quantification ∀

"∀" means "for all"

**∀xP(x)** is true **if and only if** 

**P(x1)∧P(x2)∧...∧P(xn)** 	is true



### Existential Quantification 

"∃" means "For some"

**∃xP(x)** is true **if and only if** 

**P(x1)vP(x2)v...vP(xn)** 	is true





![1559082835815](assets/1559082835815.png)





![1559083390959](assets/1559083390959.png)

**The first one and last one are one way**

Example:

∃x[P(x) ^ Q(x)] => [∃x(P(x)) ^ ∃x(Q(x))]

∃x "all student"

P(x) = x is male

Q(x) = x is female

if we say that  **[∃x(P(x)) ^ ∃x(Q(x))]**

that means:

**one of the student is male, one of the student is female**

and **∃x[P(x) ^ Q(x)]** means:

**one of the student is male and female**

it is wrong, so we can't say  **[∃x(P(x)) ^ ∃x(Q(x))] <=> ∃x[P(x) ^ Q(x)]**

 only **[∃x(P(x)) ^ ∃x(Q(x))] => ∃x[P(x) ^ Q(x)]**



###  Negation of Quantifiers

Often we use statements which are the negation of a quantification
The logical equivalent statement is defined as follows: 
$$
¬∀xP(x) = ∃x¬P(x)
$$

$$
¬∃xP(x) = ∀x¬P(x)
$$

![1559113711157](assets/1559113711157.png)

### Multiple Quantifiers

In the universe of integers:
Let P(x,y) = “x + y = 0”, then what are the truth
values of: 

1. ∀x ∃y P(x,y)
2. ∃x ∀y P(x,y) 

(1) means : For all x, there is a y , that makes x+y = 0

(2) means : There is a x, for all y, that makes x+y = 0

so (1) is true, but (2) is false.

thouse two are not equal valid

----------------------------------------

Let Q(x,y) = “x·y = y·x”, what is the truth value of:
(Ex.3-12)

1. ∀x ∀y Q(x,y)
2. ∀y ∀x Q(x,y) 

(1) means : For all x, for all y, that x·y = y·x 

(2) means : For all y, for all x, that x·y = y·x 

(1) <=> (2)

![1559114195400](assets/1559114195400.png)

![1559114579461](assets/1559114579461.png)

**Example 1:**

proof:

```
∀x(p(x) -> q(x))
∀x(q(x) -> r(x))
-----------------
∀x(p(x) -> r(x))
```

∀x(p(x) -> q(x)) is true, 

for arbitrary (任意数) element a,

p(a) -> q(a)



∀x(q(x) -> r(x)) is true,

for arbitrary element b,

q(b) -> r(b)



since b is arbitrary, b can be a,

so the fomular change to 

```
p(a) -> q(a)
q(a) -> r(a)
-----------------
p(a) -> r(a)
```

by Universal Generalization

p(a) -> r(a)	 is 	∀x(p(x) -> r(x))

------

Example 2.

proof: 

```
(1)		∀x(p(x) -> q(x))
		_________________
		∃x¬(p(x)) -> ∃x(q(x))
		
(1)		∀xp(x) -> ∀xq(x)		(2)
(2)		¬∀xp(x) v ∀xq(x)		(3)
(3)		∃x¬(p(x)) v ∀xq(x)		(4)
		if ∀xq(x) is true, then ∃x(q(x)) must be true
		so
		∃x¬(p(x)) -> ∃x(q(x))

```



### Proof of Theorems

![1559115302440](assets/1559115302440.png)

Example of proof by contradiction:

proof √2 is Irrational number(无理数)



Assume (¬p) √2 is rattional,

∃n,m; √2 = m/n	(n,m no common factor)

m = √2 n => m^2 = 2n^2

m^2 is even so m is even.

∃k, m = 2k, so

4k^2 = 2n^2

2 k^2 = n^2

n^2 is even, n is even.

so m,n both even, 2 is common factor, but n,m should no common factor

so √2 is Irrational number



Exercise:



```
1.
	¬(∀x∀y[(x<y) -> ∃z(x<z<y)])
<=>	∃x∃y¬[¬(x<y) v ∃z(x<z<y)]
<=>	∃x∃y ((x<y) ^ ¬∃z(x<z<y))
<=>	∃x∃y ((x<y) ^ ∀z¬(x<z<y))
<=> ∃x∃y ((x<y) ^ ∀z¬(x<z ^ z<y))
<=> ∃x∃y ((x<y) ^ ∀z(¬(x<z) v ¬(z<y))
<=> ∃x∃y ((x<y) ^ ∀z(x >= z V z >= y)

2.
	∀x[p(x) v q(x)]		(1)	
	∃x¬p(x)				(2)
	∀x[¬q(x) v r(x)]	(3)
	∀x[s(x) -> ¬r(x)]	(4)
	_________________
	∃x ¬s(x)

(2) there exist c in u, that ¬p(c)
(1)	p(c) v q(c)
(3)	¬q(c) v r(c)
(4)	s(c) -> ¬r(c)

so the fomular change to:
	p(c) v q(c)		(1)
	¬p(c)			(2)
	¬q(c) v r(c)	(3)
	s(c) -> ¬r(c)	(4)
	___________________
	¬s(c)

(3)		q(x) -> r(c)	(5)
(5)		¬r(c) -> ¬q(c)	(6)
(4)(6)	s(c) -> ¬q(c)	(7)
(2)(1)	q(c)			(8)
(7)(8)	¬s(c)
		∃x ¬s(x)


```





## --- Number Theory ---

### Division

a|b means there is a c, so that b = ac

3|9 	9 = 3*3



#### Theorem 1,2,3

**1)**

if	 **a|b** , **a|c**	 then	 **a|(b+c)**



proof:	a|b => ∃k1 ak1 = b

​		   a|c => ∃k2  ak2 = c

b+c = ak1+ak2 = a(k1+k2)

because k1 + k2 is integer, so a|(b+c)



**In general  	a|b 	a|c	then 	a|bx+cy 	for any integer**



**2)**

if	 **a|b** 	then	 **a|bc**	 for all integers c



**3)**

• if 	a|b	 and 	b|c,	 then 	a|c



proof:

​	a|b => ∃k1 b = ak1

​	b|c => ∃k2  c = bk2

​	c = ak1k2	k1*k2 is integer

​	so  a|c



### Prime Number 质数

定义:

​	A positive integer greater than 1 is called prime if
​	the only positive factors of p are 1 and p.
​	Otherwise, it is called composite. 

prime : 13, 7

composite: 12, 9



#### Well Ordering Primcipal

If you have a collection of positive integers, then that collection has a least element



##### Theorem4:

If m is an positive integer, and m is compositive

then there exist p, p is prime number such that p|m



proof:

​	if there is a collection (n1, n2, n3 ....) such that is false (they are all comositive, and the don't have prime factor)

​	by **WOR** ∃n such that n < ni, 

​	∃n1n2;	n = n1*n2

​	=> n1 < n ^ n2 < n

​	n1, n2 are not prime since n

​	n1^ n2 are compositive

​	n1 < n, n2 < n since n is the least element

​	n1 is not in that collection, therefore 

​	∃p; p|n,

​	p|n1 ^ n1 | n => p|n	**contradiction**



##### Theorem 5: 

There are infiniteley many prime numbers

proof: 

​	Assume the total number of prime numbers are finite	p1, p2, p3... pn

​	a = p1 * p2 * p3 * ... * pn + 1

​	since a > pi, 	a is composite

​	∃p such that p|a

​	pi | a

​	pi | p1 * p2 ... pn

​	so pi | (p1 * p2 ... pn +1) - (p1 * p2 ... pn) 

​	pi | 1

​	pi = 1

​	1 is not prime number, comtradiction

##### **Theorem 6:**

If n is a composite integer, then n has a prime
divisor less than or equal to ![1559966922116](assets/1559966922116.png)

proof:

​	n is composite 	∃m1m2

​	n = m1 * m2

​	m1 > ![1559966922116](assets/1559966922116.png) 	^	 m2 > ![1559966922116](assets/1559966922116.png)

​	m1m2 > ![1559966922116](assets/1559966922116.png)*![1559966922116](assets/1559966922116.png)

​	¬(m1 > ![1559966922116](assets/1559966922116.png) )	v 	¬( m2 > ![1559966922116](assets/1559966922116.png))

​	Assume m1 <  ![1559966922116](assets/1559966922116.png)

​	m1 is compositive 	p | m1

​	

​	m1 | n	p | m1

​	so p | n



### gcd and lcm

gcd greatest common divisor

lcm least common multiple



#### Theorem 7:

if a>b then gcd(a,b) = gcd(a-b, b)



proof:

​	gcd(a,b) = d1

​	gcd(a-b,d) = d2

​	d1|a ^ d1|b	=> d1|ax+by => d1|a-b ^ d1|b	=> d1|d2	(because d2 is greatest)

​	d2|a-b ^ d2|b

​	d2|(a-b) + b => d2|a	=> d2|d1 (d1 is greatest)

​	because d1|d2 ^ d2|d1	d1 == d2



#### Theorem 8 :

​	if a,b,c are positive integers, the diophuntine equation ax+by=c has an integer solution (x0, y0)

​	if and only if gcd(a,b)|c



#### Theorem 9:

​	let a, b be positive integer, p is prime number

​	if p|ab then p|a or p|b

​	

proof:

if p | a then Done	

else gcd(p,a) = 1

since gcd(p,a) = 1, c=1

px+ay=1 has a integer solution	(by Theorem 8)

pbx+aby=b 

because p|ab so let ab = pk

pbx + aby = b =>	pbx + pky = b

so then p|b



#### theorem 10:

ab = gcd(a,b)*lcm(a,b)



### modular

Let a be an integer and m be a positive integer.
The remainder when a is divided by m is denoted
a mod m.

a mod m = r 	a=mq+r 	0<=r<m



a≡b (mod on m)	m | a-b



#### Theorem 11:

if 	a≡b(mod on m) and c≡d(mod on m)

then	a+c≡b+d (mod on m)	ac≡bd(mod on m)



#### Theorem 12:

a = bq+r

gcd(a,b) = gcd(b, r)



Example 

gcd(a, b) = 1	if a|bc	proof a|c

ax+by=1 (c=1) has a integer solution 

ax0+by0 = 1

acx0+bcy0 = c

because a|bc

a|acx0 and a|bcy0

so a|(acx0+bcy0)

​	a|c(ax0+by0)

​	a|c*1

​	a|c



Example

gcd(a,b)=d

show gcd(a/d, b/d)=1



ax+by=d has a integer solution

∃x0y0

ax0+by0=d

(a/d) x0 +(b/d) y0 = 1

so gcd(a/d,b/d)=1



Example:

2^1234 ≡ ? (mod on 17)

2^4 = 16 ≡ -1 (mod on 17)

2^8 ≡ 1 (mod on 17)

2^8^154  *  2^2 ≡1 * 2^2 (mod on 17)

so ? = 4



example:

为什么3的倍数,各项之和也是3的倍数

n = a0 * 10^0 + a1 * 10 + ... + an * 10^n

10 ≡ 1(mod on 3)

so a0 * 1 + a1 * 1 ... + an * 1 



## ---Set Theory---

### set :

S = {}

A = {2,3,4}

∈ means belongs to
∉   means not belongs to

2 ∈ A 	99  ∉ A



empty set: {} or ∅ 

### set builder:

A = {2k | 0<k<5, k: integer}

​		

### size of set

|A| = 3	size of A

Important Set

![1560638908820](assets/1560638908820.png)



### sub Set

A is a sub set of B

A ⊆ B

∀x(x ∈ A-> x ∈ B)

```
		¬∀x(x ∈ A-> x ∈ B)
<=>		∃x ¬( ¬(x ∈ A) v (x ∈ B))
<=>		∃x (x ∈ A) ^ (x ∉ B)
```



#### same set:

A = B iff A ⊆ B ^ B ⊆ A

#### proper Subset:

A ⊂ B

1. ∀x(x ∈ A-> x ∈ B)

2. ∃x (x ∈ B) ^ (x ∉ A)



### Theorem 1

A ⊆ B ^ B ⊆ C	=>	A ⊆ C

```
because A ⊆ B
so 		∀x(x ∈ A -> x ∈ B)

because B ⊆ C
so		∀x(x ∈ B -> x ∈ C)

so we need to proof:
∀x(x ∈ A -> x ∈ B)
∀x(x ∈ B -> x ∈ C)
___________________
∀x(x ∈ A -> x ∈ C)

use arbitrary a 

x ∈ A -> x ∈ B
x ∈ B -> x ∈ C
________________
x ∈ A -> x ∈ C
```

### Theorem 2

If A ⊂ B and B ⊆ C then A ⊂ C

proof:

1. ∀x(x ∈ A -> x ∈ C)

2. ∃x (x ∈ C ^ x ∉ A)

```
by:
A ⊆ B ^ B ⊆ C 	=>	A ⊆ C
we got ∀x(x ∈ A -> x ∈ C)

because A ⊂ B 
so		∃x(x ∈ B ^ x ∉ A)
because B ⊆ C
		x ∈ B => x ∈ C
		x ∈ C ^ x ∉ A
```



### Theorem 3

A be a set in a given universe U, then {} ⊆ A. Also, if A!={} then {} ⊂ A

1. ∀x(x ∈ {} -> x ∈ A)

   x ∈ {} is false so the whole statement is true

2. if A != {} => {} ⊂ A

   {} ⊆ A  is  true

   ∃x(x ∈ A ^ x ∉ {})

   a is a arbitrary element in A

   A != {} -> a ∈ A

   A has at least 1 element

   a ∈ A ^ a ∉ {}	=>	∃x(x ∈ A ^ x ∉ {})	true





### Power Sets

Given a set A in a given universe U, a power set of
A is the set of all possible subsets of the set A. It is
denoted by P(A).



Example:

A = {1,2}

P(A) = {{}, {1}, {2}, {1,2}}

|P(A)| = 2^2 = 4



if	|A| = n then |P(A)| = 2^n

(n choose 0) +(n choose 1) ... (n choose n) = 2^n



### Theorem 4:

(n+1 choose r) = (n choose r) + (n choose r-1)



proof:

A = {a1, a2, a3 ... an, b}

(n+1 choose r) select r element from A

1. not include b, select r from ai (n choose r)
2. include b, select r-1 from ai (n choose r-1)

```
						1
					1		1
			
            	1		2		1
				(3 c 1)	  (3 c 2)
			1		3		3		1
					  \	  /
		1		4		6		4		1
					 (4 c 2)
```



### Set Operations

![1560645235256](assets/1560645235256.png)

![1560645347749](assets/1560645347749.png)

![1560645439887](assets/1560645439887.png)

![1560645502553](assets/1560645502553.png)





### Theorem 5:

if A, B are sets in a universe U, then A and B are disjoint iff AUB = A△B

​		    iff

A ∩ B = {}  <=> A U B = A△B

because A U B = A△B

1. A U B ⊆  A△B
2. A△B ⊆  A U B      -> always true



by 1

a ∈ AUB

a ∈ AUB ^ a ∉ A ∩ B

so a ∈ AUB 





### Theorem 6

1. A ⊆ B

2. A U B = B

3. A ∩ B = A

4. __	__

​        B   ⊆   A

 

proof (3)(4)

!B means not in B

¬ ∀ ∃ ∈ ∉ ⊆ △ ∩

```
a ∈ !B => a ∉ B => a ∉ A ∩ B
!A = {x| x ∈ U ^ x ∉ A }
A ∩ B = A 	=>	a ∉ A => a ∈ !A

Assume
!B ∉ !A
there exist c;
c ∈ !B ^ c ∉ !A
focus on c ∉ !A
=>	c ∈ A
	because A = A ∩ B
=>	c ∈ A ∩ B
=>	c ∈ B	but c ∈ !B
	contradiction
```



Example:

show

!!A = A

so we need to proof:

1. !!A ⊆ A

2. A ⊆ !!A

   !!A ⊆ A	<=>	a ∈ !!A 	<=>	a ∉ !A	<=>	a ∈ A



Example:

simplfy !(A △ B)

!(A △ B)	=>	!((A U B) - (A ∩ B))

​		because A - B = A ∩ !B

​		     =>	!((A U B) ∩ ! (A ∩ B))

​		     =>	!(A U B) U (A ∩ B)

​		     =>	 (!A ∩ !B) U (A ∩ B)

​		     =>	!A ∩ ((!B U A) ∩ (!B U B))

​		     =>	!A ∩ (!B U A)

​		     =>	(!A ∩ !B) U (!A ∩ A)

​			=>	!A ∩ !B

Example:

proof :	A ⊆ B iff A ∩ !B = {}

​		

```
1. proof A ∩ !B = {}	=>	A ⊆ B

	a ∈ A 
=>	a ∉ !B
=>	a ∈ B
=>	A ⊆ B

2. proof A ⊆ B 	=>	A ∩ !B = {}
	assume (A ∩ !B) != {}
	c ∈ (A ∩ !B)
=>	(c ∈ A) ∩ (c ∈ !B)
because c ∈ A and A ⊆ B
so		c ∈ B
because c ∈ !B
so		c ∉ B	contradiction
```



