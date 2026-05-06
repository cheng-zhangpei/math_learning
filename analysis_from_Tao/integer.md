## 整数的定义

对于整数的定义似乎一开始，我们是想要以减法作为触发去进行定义，但是现在我们还没有定义减法所以采用加法来定义。a—b定义为整数，这里的—只是一个占位符不代表减法，但是用加法来定义a—b=c—d，这个等号只有在a + d = c + b这个基础上成立。、

然后我们要验证啥？验证整数相等是一个合理的概念，这个时候我们转向去验证自反性、对称性、传递性。自反性和传递性是习题，我们现在验证传递性。我们现在有两个式子$a—b=c—d$、$c—d=e—f$现在这两个式子可以推出：$a+d=c+b$、$c+f=e+d$。这两个式子相加可得
$$
a+d+c+f=c+b+e+d\\
a+f=b+e\\
a—b=e—f
$$
这就说明有传递性了。

> 为啥我们要用减法去定义整数，是因为对于自然数系而言3-5没法在自然数系中进行表示，所以我们需要一个更大的数系将3-5这种给包裹进去
>
> 一个很自然的想法是，用两个自然数的"差"来表示一个新数。
>
> => 所以数据的创建往往是为了弥补之前数系的缺陷而被创造的

![image-20260503143858012](C:\Users\czp13\AppData\Roaming\Typora\typora-user-images\image-20260503143858012.png)

这是判断这个定义是否成功的一个方法，也就是等量替换后，可以证明相等。这些式子的具体证明还是要转为整数最开始的相加的定义，然后将已知条件代入就好了。

**整数的负数定义**：如果a-b是一个整数那么b-a记作a-b的的负数，记作-(a-b)。这个如何证明-> 习题

**整数的三歧性：**
$$
x>0 \lor x<0 \lor x=0 \quad
$$
三歧性不是在告诉你"正、负、零"这三个概念是什么，而是在保证：整数的世界里没有"灰色地带"，每个数都必然落在某一个明确的类别里。三歧性的证明是分为两个大点：

- 正确性：首先我要证明每一点都是对的也就是对于一个整数x = a-b满足上面三个式子，那么我们就分为a>b\a<b\a=b去进行讨论。

- 唯一性：我们只要去假设这三个式子里面有两个式子是成立的去用一个式子去证明另外一个式子有问题，诶这不就是反正法吗？

> 这里遇到一个概念就是交换环的概念，这个概率是抽象代数里面的东西，环的本质是一系列规则的系统，规则如下：
>
> ```
> ① 加法交换律      a + b = b + a
> ② 加法结合律      (a+b)+c = a+(b+c)
> ③ 零元            a + 0 = a
> ④ 相反数          a + (-a) = 0
> ⑤ 乘法结合律      (a×b)×c = a×(b×c)
> ⑥ 分配律          a×(b+c) = a×b + a×c
> 而交换环其实就是相比于其他的环多了一个乘法加法交换律：
> （2×(3+4) = 2×3+2×4）
> ```

所有的整数构成一个交换环。

![image-20260503171857779](C:\Users\czp13\AppData\Roaming\Typora\typora-user-images\image-20260503171857779.png)

这俩题就在习题里面做就是了。今天晚上看看习题就好了

----

## 习题

1: Verify that the definition of equality for integers is reflexive or symmetric.

So We should at least understand what is Refexivity and Symmetry.

Refexivity: let a and b be nature number,and a — b is an integer, for the nature number we have a + b = a + b, so that we have a — b have the same quality which the equation, so a—b = a—b (it is a little bit wired)

Symmetry: 
$$
prove:a—b = c—d\\\iff c—d=a-b
$$
answer: $a—b=c—d \iff a+d=c+b \iff c+b=a+d \iff c—d = a —b$ 

2: we have$(a-b)=(a^{\prime}-b^{\prime})$，prove $-(a-b)=-(a^{\prime} - b^{\prime})$

prove:
$$
\begin{align}

-(a—b)=b—a\\-(a^{\prime} - b^{\prime})=b^{\prime}—a^{\prime}\\
prove:b—a=b^{\prime}—a^{\prime}\\
\iff b+a^{\prime}=b^{\prime}+a\tag{1}\\
\because a—b=a^{\prime}-b^{\prime}\\
\therefore a + b^{\prime}=a^{\prime}+b\tag{2}
\\ from (2)\iff (1)
\end{align}
$$
So this problem is proved.

3: we have a integer a, prove $(-1) \times a=-a$

> we have the definition of the multiple operation: 
>
> $(a—b) \times (c—d) = (ac+bd)-(bc+ad)$

prove:
$$
(-1) \times a = -a \iff (0-1)\times(a-0)=-a
$$
Just a simple equation can finished the process of the prove.

4: Prove, Let x and y two integer, make $xy = 0$,so that $x=0\lor y=0 \lor x=y=0$.

prove: 

The trichotomy offer a nature classification framework of a single number. So we can use trichotomy to divide the x into 3 different classifications. $y=c-b$,with c,b nature numbers.

1. x=0,that is obvious right,fit the equation we wanna prove
2. x > 0,  If x > 0, we can set x = n-0($n\neq0$), n is a nature number. $\because xy=0$, $\therefore (n-0) \times(c-b)=nc-nb=0$, so we have nc = nb, we can use the cancellation law of the nature number$\therefore c=b,y=0$.
3. x<0, it is the same with the 2

Actually, I feel like the proof for this problem is a little off.



