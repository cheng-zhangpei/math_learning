# Absolute Value and Exponential Operations

> I’ve realized there’s a serious problem: from now on, even if I can’t solve a problem, I’m going to force myself to think about it for 10 to 15 minutes—otherwise, doing the exercises will be a waste of time.

1) prove proposition 4.3.3(I do not have time to prove all of them)

let set the x and y are national numbers.

a)  $|x| \geq 0$ and only when x=0 ,$|x|=0$

let set x is rational number, if x > 0, we have |x|=x, if x < 0 |x| = -x , |x| > 0, x=0,|x| = 0. according to the trichotomy  of rational number, x can only be one of them, so only when x = 0, we have |x| = 0.

 b) $|x+y|\leq|x|+|y|$

> let set x and y are rational numbers. let us try to fix y and classify x:
>
> when x > 0, we have $|x+y|$,  
>
> if we just classify one variant, you would figure out can not keep on, so we should classify two variants at the same time.

the answer do not have one variant is 0, the other is not. and we should discuss a lot classifications....

(1) we have x >0 and y > 0, |x + y| = |x| + |y| 

(2) we have x < 0 and y < 0, |x + y| = -(x + y) < 0 < |x| + |y|

(3) we should discuss x < 0 and y > 0 or x > 0 and y < 0, they are actually the same. 

on one hand , x > 0 and y <0, |x| + |y| = x - y > 0, x > y.

on the other hand , if we regard the |x + y| as a combination, we have |x + y| = x + y

ok, in this case, we can combine these situations, y is negative, we have |x+y| = x + y < x - y = |x| + |y|.  in conclusion, all the case is prove.

c) |xy| = |x| |y|, especially when |-x| = |x|

> it is the same, we have 4 different situations, we should take the sign of x and y into consideration

(1) x = 0, and y = 0. |xy| = 0 = |x| |y| = 0

(2) x > 0 and y > 0. |xy| = xy, and |x| |y| = xy , so |xy| = xy

(3) x < 0 and y < 0 |xy| = |-(-x)(-y)| = (-x)(-y), |x| |y| = (-x)(-y), so |xy| = |x| |y|.

(4) if x and y have reverse sign, we suppose x > 0 and y < 0(the opposite case is the same stuff). for |x||y| = x (-y) > 0, for |xy| = |-x(-y)|,and x(-y) > 0, so we have |xy| = x(-y). so we proved |xy| = |x||y|

2. prove proposition 4.3.7

> it is the same, I will just pick some of them to prove, it is hard for me to prove all of them.

a) if x = y, for any $\varepsilon>0$, we have x access to y with $\varepsilon-$, and prove the reverse.

let set x and y are rational numbers. 

(1) forward: $d(x,y) < \varepsilon$, and $\forall \varepsilon$,because x = y ,so $d(x,y)=0$, and for $\forall \varepsilon>0$, so d(x,y) < 0 holds for any

(2)backward(**using contradict, a little bit hard**):  consider the contradiction, and $d(x,y)<\varepsilon, x\neq y$, assume $\varepsilon=|x-y|/2$, so we have $|x-y|>0,\varepsilon$ is a positive number, so we have d(x ,y) = $\varepsilon + \varepsilon > \varepsilon$ , which is a contradiction.

> this is a Proof Of Contradiction, we should consider that carefully.

d)set $\var,\varepsilon>0$, if x and y is $\varepsilon-$access, while z and w is $\var$ access,so x+z and y + w is ($\var + \varepsilon$)- access, and x-z, y-w is also  ($\var + \varepsilon$)-  access

let set x, y, w and z is rational numbers, and x > y

(1) d(x,y) <  $\varepsilon$ , let set x - y = a(|a| < $\varepsilon$). the same we have d(z,w) < $\var$, let us set z - w = b (|b| < $\var$).

|x - z| = |a + y - b - w|, |(x-z) - (y-w)| = |a + b| <($\varepsilon$ + $\var$)

(2) d(x + z, y + w) = |(x + z) - (y + w)| =|(x-y) + (z-w)|$\leq$|x-y| + |z-w| $\leq$ ($\varepsilon$ + $\var$)

(1) and (2) actually just prove one thing.

---



3. prove proposition 4.3.10

(a) prove, $x^mx^n=x^{m+n}$, $(x^n)^m=x^{nm},(xy)^n = x^ny^n$

firstly, the framework of  Induction should appeal in my mind,  you should fix one variant and do the induction in the other. 

let set m = 0, so $x^0x^n = x^n$, that is right obviously,so we hypothesis that $x^mx^n = x^{m + n}$ is correct. we should prove $x^{m+1}x^n = x^{m+n+1}$

$x^{m+1}x^n = (x^mx)x^n=x^mx^nx = x^{m+n}x = x^{m+n+1}$

> we  always use the definition: $x^{n+1} = x^n \times x$, The rest of the approach is the same, so I won’t go into detail here.

4. for any positive integer N, we all have $2^N > N$

> how can we know use induction?

​    Let set N = 1 , So we have 2 > 1, Now suppose that inductively $2^N > N$

we wanna prove: $2^{N+1} > N+1$

$2^{N+1} = 2^N 2>2(N) \geq N + 1$(we Know $N \geq1$)

so we have $2^{N+1} > N+1$

