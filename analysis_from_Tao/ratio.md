# rational number

## Title

1. Prove that the definition of rational numbers Reflexivity, symmetric, and Transitivity.
2. Proof of several equations of 4.2.4
3. Proof of Lemma 4.2.7(*trichotomy of rationals*)
4. Proof of Proposition 4.2.9
5. Prove that if x, y, and z are rational numbers such that x < y and z is negative, then xz > yz.

-----

## Answer

1.

a. Reflexivity: we just need to prove that $a//b=a//b$, we can convert the equation to $ab=ba$ , using the reflexivity of equality on Z,we can prove the Reflexivity

> why we use  $ab=ba$, actually, there is no differences, you can use ba or ab, the equation is always right. 

b. symmetric: for symmetric, we should prove the equation: $a//b=c//d \iff c//d=a//b$, so we can convert the left equation to $ad=cb(1)$, for right equation can convert to $cb=ad(2)$, it is obvious (1) == (2)

c. Transitivity: we should prove $a//b=c//d,c//d=e//f \iff a//b=e//f$, the same start with converting to the Multiplication equation, so we have to prove $ad=bc(3),cf=de(4) \iff af=eb$,we should try to find the connection between between (3) and (4), for (3),can multiply e in both side,we have $ade=bce \iff acf=bce$,we can use the cancellation law, we get $acf=bce\iff af=be$

---

2.

I just pick of the equations to prove:

<img src="C:\Users\czp13\AppData\Roaming\Typora\typora-user-images\image-20260509113222004.png" alt="image-20260509113222004" style="zoom:50%;" />

We have x\y\z, let us set $x=a//b,y=c/d,z=e/f$, all the variants is the rational number.

a. 
$$
left:x+y=a//b + c//d \iff \frac{ad+bc}{bd}(1) \\
right:y+x=c//d+a//b \iff \frac{cb+ad}{db}(2)
$$
we can use the commutativity of addition and multiplication of integer. obviously, (1) equals to (2)

b. 

the same with a, I do not wanna spend too much time.

c.

we should use the a to assist, $x+0=0+x$,we can get this equation from a.$x+0=a//b+0//n=\frac{an+b0}{bn}=a//b=x$

d.

The proof essentially follows the same approach of finding a common denominator, so there’s really no difference.

----

3.

proof: $x>0\lor x=0 \lor x<0$(only one true)

proof of trichotomy have been seen for many times... What is the essential of this kind of problem? We should divide the proof into two parts,1) proof at least one of the statement is true. 2) proof only one of the statement is true(can not exist two different statements)

1)We Set the x = $a//b,b\neq 0$,with a,b integers. if $a=0,x=0$ is true  obviously, for a and b,both of them have negative and positive situation,so that we can consider the situation separately.

- $a>0,b>0\iff x > 0$
- $a>0,b<0\iff x<0$
- $a<0,b<0\iff x>0$
- $a<0,b>0\iff x<0$

> If $a,b$ are natural numbers, we need to define positive and negative values more explicitly; however, since the set of integers is also a commutative ring, I don’t think it’s necessary to define natural numbers.

2)We also try to combine 2 of 3 statements, try to find contradiction.

- suppose $x>0\land x = 0$,$x>0\iff (a>0,b>0)\lor(a<0,b<0)$, if $x=0$,we have $a=0$,owing the trichotomy of integers, $x>0\quad and\quad x = 0$ are mutually exclusive. 
- the same with $x<0\land x = 0$
- suppose $x>0 \land x<0$, if both of the statements should be fulfilled, which means that we should have the equation $x=c//d=(-n)//m$, with c,d,n,m a positive nature numbers.  so we have $-nd=cm$, a positive number can never be equal to a negative number.

In conclusion, 1) at least one of the statement is true. 2)  only one of the statement is true(can not exist two different statements)

---

4.

Let *x, y, z* be rational numbers. This proposition includes the following statements:

a) Prove that exactly one of the three statements $x>y$,$x<y$,$x=y$ is true. 

The essence of this proof is $x>y \iff x-y>0$,We can know $x-y$ is a integer, by using the trichotomy of the integer, we will have the statements if true

 b)Prove that one has $x>y$ if and only if $y<x$.

let  $x=a//b,y=c//d$,with $a,b,c,d$ positive nature number. $x-y=x+(-y)=(ad-bc)//bd$, if $y<x$,we have $bc-ad<0\iff ad > bc$, so the $x>y$

> we can also set $x-y=n//m$, the method is the same.

c)Prove that if $x<y$, then $x+z<y+z$.

> notice: We cannot use transposition as part of the proof, because we have not yet proven that transposition preserves inequalities! We can only use known mathematical definitions to prove it.

we have $x-y=(x+z)-(y+z)<0\iff x+z<y+z$

d)Prove that if $x<y$ and *z* is positive, then $xz<yz$.

$x<y\rightarrow x-y<0 \rightarrow z(x-y)<0\rightarrow zx-zy<0\rightarrow xz <yz$

because z is positive and $x-y$ is negative, $z(x-y)$ is negative.(we prove that in the book). But I will try to repeat the proof process:

> we set $x=a//b,y=(-c)//d$. with a,b,c,d is positive nature number. so we have $x>0,y<0$. $x \times y=-(ac)//bd$, $bd$  is positive and ac is positive ,so we have $x\times y$ is negative.  

---

5.

*Show that if* *x, y, z* *are rational numbers such that* *x* > *y* *and* *z* *is negative,*then xz > yz

We also let  $x-y<0,z<0\rightarrow (x-y)\times z > 0 \rightarrow xz-yz>0 \rightarrow zx>yz$