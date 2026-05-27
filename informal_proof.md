---
title: A Generalization of the Lindeberg Principle
author: Sourav Chatterjee
journal: The Annals of Probability, 2006, Vol. 34, No. 6, 2061--2076
doi: 10.1214/009117906000000575
---

# A Generalization of the Lindeberg Principle

**Sourav Chatterjee**  
*University of California, Berkeley*

> *The Annals of Probability*, 2006, Vol. 34, No. 6, 2061--2076.  
> DOI: `10.1214/009117906000000575`.  
> © Institute of Mathematical Statistics, 2006.

## Abstract

We generalize Lindeberg's proof of the central limit theorem to an invariance principle for arbitrary smooth functions of independent and weakly dependent random variables. The result is applied to get a similar theorem for smooth functions of exchangeable random variables. This theorem allows us to identify, for the first time, the limiting spectral distributions of Wigner matrices with exchangeable entries.

## 1. Introduction and results

J. W. Lindeberg's elegant proof of the central limit theorem [12], despite being in the shadow of Fourier analytic methods for a long time, is now well known. It was revived by Trotter [20] and has since been successfully used to derive CLT's in infinite-dimensional spaces, where the Fourier analytic methods are not so useful.

While the original Lindeberg method and its extensions compare the distributions of convolutions in great generality (the history of which is irrelevant to our discussion, so we refer to [15] for details), it soon becomes clear that the same principle works not only for sums, but for more general smooth functions as well. Comparison of $f(X_1,\ldots,X_n)$ and $f(Y_1,\ldots,Y_n)$ for polynomial $f$ has been examined by Rotar [16] and Mossel, O'Donnell and Oleszkiewicz [13], and for general smooth $f$ with bounded derivatives by Chatterjee [5]. In [5], it is shown how to apply the method to establish universality in physical models, including the Sherrington--Kirkpatrick model of spin glasses. It was recently observed by Toufic Suidan [18] that the results in [5] can be used to give an immediate proof of the universality of last passage percolation in thin rectangles (originally a result of [3] and [4]). Developed independently, the Mossel, O'Donnell and Oleszkiewicz paper [13] is another repository of very striking modern applications of this very old idea.

A closer examination of Lindeberg's method reveals that there is a direct generalization by which the independence of the coordinates can be dispensed with. The argument, which may be possible to guess once the theorem has been stated, will be given in Section 2.

**Received** August 2005; revised March 2006.  
**Supported in part by** NSF Grant DMS-04-06042.  
**AMS 2000 subject classifications.** Primary 60F17; secondary 60G09, 15A52.  
**Key words and phrases.** Lindeberg, de Finetti, Wigner, exchangeable, random matrices, invariance principle, semicircle law.

### Theorem 1.1

Suppose $X$ and $Y$ are random vectors in $\mathbb{R}^n$ with $Y$ having independent components. For $1 \le i \le n$, let

$$
A_i := \mathbb{E}\left|\mathbb{E}(X_i\mid X_1,\ldots,X_{i-1})-\mathbb{E}(Y_i)\right|,
$$

$$
B_i := \mathbb{E}\left|\mathbb{E}(X_i^2\mid X_1,\ldots,X_{i-1})-\mathbb{E}(Y_i^2)\right|.
$$

Let $M_3$ be a bound on $\max_i(\mathbb{E}|X_i|^3+\mathbb{E}|Y_i|^3)$. Suppose $f:\mathbb{R}^n\to\mathbb{R}$ is a thrice continuously differentiable function, and for $r=1,2,3$, let $L_r(f)$ be a finite constant such that $|\partial_i^r f(x)|\le L_r(f)$ for each $i$ and $x$, where $\partial_i^r$ denotes the $r$-fold derivative in the $i$th coordinate. Then

$$
\left|\mathbb{E}f(X)-\mathbb{E}f(Y)\right|
\le
\sum_{i=1}^n\left\{A_iL_1(f)+\frac12 B_iL_2(f)\right\}
+\frac16 nL_3(f)M_3.
$$

Let us now say a bit about the condition of boundedness of third derivatives. The implications of this condition have been inspected in detail in the context of convolutions by Zolotarev (see, e.g., [23]) and other authors. Zolotarev defines the $\zeta_3$-metric on the space of distributions as follows: $\zeta_3(F,G)=\sup_f|\int f\,dF-\int f\,dG|$, where the sup is taken over all $f$ with third derivative bounded by 1. The $\zeta_3$ metric has not been so popular in practice because of the difficulty in connecting this metric with the common notions of distance between measures.

However, instead of taking supremum over a class of $f$'s, we consider only individual functions of interest. For instance, in the random matrix scenario, our $f$ will be the Stieltjes transform of a matrix at a fixed $z\in\mathbb{C}\setminus\mathbb{R}$, which is a nice $C^\infty$ function of the original matrix. In the paper [5], the author considered the partition function of a disordered physical system (the Sherrington--Kirkpatrick model of spin glasses), which again turns out to be a $C^\infty$ function of the disorder matrix, and has nicely bounded derivatives.

The condition of boundedness of the derivatives can be dropped (as demonstrated in [16] and [13]) by careful examination of the remainder term; but our focus is different: We are more concerned with ways to extend the method to the case of weakly dependent variables (as in Theorem 1.1 above), and more specifically, to exchangeable random variables, as below.

### Exchangeable random variables

Let us now present a surprisingly nontrivial application of the basic tool developed in the previous section. Suppose $X$ is a vector with exchangeable components. Certainly, we cannot expect to replace the components of $X$ by independent Gaussians as we did in Theorem 1.1. For instance, all the components may be equal to the same random variable, in which case there is no hope of replacing these variables by something generic. However, not all is lost; our next theorem shows that the following "summarization" of $X$ can still be carried through:

Suppose $X$ is a vector with exchangeable components, having finite fourth moments. Let

$$
\hat\mu := \frac1n\sum_{i=1}^n X_i
\quad\text{and}\quad
\hat\sigma^2 := \frac1n\sum_{i=1}^n (X_i-\hat\mu)^2. \tag{1}
$$

Let $Z$ be a standard Gaussian vector in $\mathbb{R}^n$, independent of $X$. Let $\bar Z:=n^{-1}\sum_{i=1}^n Z_i$ and

$$
Y_i := \hat\mu+\hat\sigma(Z_i-\bar Z),\qquad i=1,\ldots,n. \tag{2}
$$

Then, for sufficiently well-behaved $f$ (to be described below), we have $\mathbb{E}f(X)\approx\mathbb{E}f(Y)$. That is, $X$ can be "replaced" by the modified vector $Y$ for evaluation under suitably smooth $f$. Note that in the process, we summarized the random vector $X$ into the couple $(\hat\mu,\hat\sigma)$. The precise statement is as follows:

### Theorem 1.2

Suppose $X$ is a random vector with exchangeable components, and $\hat\mu$, $\hat\sigma$ and $Y$ are defined as in (1) and (2). Let $f:\mathbb{R}^n\to\mathbb{R}$ be a thrice continuously differentiable function, and for $r=1,2,3$, let $L'_r(f)$ be a uniform bound on all $r$th partial derivatives of $f$, including mixed partials. For each $p$, let

$$
m_p=\mathbb{E}|X_1-\hat\mu|^p.
$$

Then we have the bound

$$
\left|\mathbb{E}f(X)-\mathbb{E}f(Y)\right|
\le 9.5\,m_4^{1/2}L'_2(f)n^{1/2}+13m_3L'_3(f)n.
$$

We postpone the (somewhat long) proof of this theorem until Section 3, giving only a brief sketch at this point. The first step is to show that there is no loss of generality in assuming that $\hat\mu\equiv0$ and $\hat\sigma\equiv1$. Having assumed that, if we define

$$
R_i=X_i+\frac{1}{n-i+1}\sum_{j=1}^{i-1}X_j,
$$

then it is a straightforward exercise (which we will work out, nevertheless) that $\mathbb{E}(R_i\mid\mathcal{F}_{i-1})=0$, where $\mathcal{F}_{i-1}$ is the sigma-algebra generated by $X_1,\ldots,X_{i-1}$. The next step is to prove

$$
\mathbb{E}(R_i^2\mid\mathcal{F}_{i-1})=1+O\left((n-i+1)^{-1/2}\right),
$$

which is computationally slightly harder. Having established these approximations, we can now replace $R_i$'s by independent Gaussian variables $V_1,\ldots,V_n$, using Theorem 1.1. However, the inverse transform, which takes $R$ to $X$, does not take $V$ to $Y$ or anything resembling $Y$, but to something that is close to $Y$ in distribution. This will be formalized using Gaussian interpolation techniques.

Before moving on to applications, let us quickly mention without detailed justification that Theorem 1.2 has no apparent connection with de Finetti's theorem [6] or its finite version due to Diaconis and Freedman [8].

### An application: Wigner's law for exchangeable random variables

Let us begin with a very quick introduction to some necessary material from random matrix theory.

#### Spectral measures

The empirical spectral distribution (ESD) of an $N\times N$ square matrix $A$ is the probability distribution $N^{-1}\sum_{i=1}^N\delta_{\lambda_i}$, where $\lambda_1,\ldots,\lambda_N$ are the eigenvalues of $A$ repeated by multiplicities, and $\delta_x$ denotes the point mass at $x$. The weak limit of a sequence of ESDs is called the limiting spectral distribution (LSD) of the corresponding sequence of matrices. The existence and identification of LSDs for various kinds of random matrices is one of the main goals of random matrix theory. For a Hermitian matrix, the ESD is supported on the real line and hence has a corresponding cumulative distribution function. We will denote the c.d.f. for the ESD of a Hermitian matrix $A$ by $F_A$. Explicitly,

$$
F_A(x)=\frac1N\#\{i:\lambda_i\le x\}.
$$

#### Wigner matrices

A standard Gaussian Wigner matrix of order $N$ is a matrix of the form $A_N=(N^{-1/2}X_{ij})_{1\le i,j\le N}$, where $(X_{ij})_{1\le i\le j\le N}$ is a collection of i.i.d. standard Gaussian random variables, and $X_{ij}=X_{ji}$ for $i>j$. Wigner [21] showed that the LSD for a sequence of standard Gaussian Wigner matrices (with order $N\to\infty$) is the semicircle law, which has density $(2\pi)^{-1}\sqrt{4-x^2}$ in the interval $[-2,2]$.

It was later shown that the distribution of the entries does not play a significant role; convergence to the semicircle law holds under more general conditions (cf. [1, 2, 10]). The weakest known condition was given by Pastur [14]. It is claimed that the condition was shown to be necessary by Girko [9]. Although most conditions require independence of the entries on and above the diagonal, there have been some advances (e.g., [7, 17]) allowing certain kinds of dependence. However, none of these cover the case of exchangeable entries.

For a detailed exposition of the key results about the spectra of Wigner matrices and other results in the study of the spectral behavior of large random matrices, see [2] or [11].

Here we consider the question of identifying the limiting spectral distributions for Wigner matrices with exchangeable entries. The following theorem gives a precise answer under minimal assumptions.

### Theorem 1.3

Suppose that for each $N$ we have a random matrix $A_N=(N^{-1/2}X^N_{ij})_{1\le i,j\le N}$, where the collection $(X^N_{ij})_{1\le i\le j\le N}$ is exchangeable and $X^N_{ij}=X^N_{ji}$ for $i>j$. Let

$$
\hat\mu_N:=\frac{2}{N(N+1)}\sum_{i\le j\le N}X^N_{ij}
\quad\text{and}\quad
\hat\sigma_N^2:=\frac{2}{N(N+1)}\sum_{i\le j\le N}(X^N_{ij}-\hat\mu_N)^2.
$$

Assume that $\hat\sigma_N>0$ a.s. for all $N$ and

$$
\sup_{N\ge1}\mathbb{E}\left|\frac{X^N_{11}-\hat\mu_N}{\hat\sigma_N}\right|^4<\infty.
$$

Then the empirical spectral distribution of $\hat\sigma_N^{-1}A_N$ converges weakly to the semicircle law in probability.

We will derive the above result from a quantitative bound (Lemma 4.1) on the difference between Stieltjes transforms (to be discussed in Section 4). The proof will show that it is actually enough to assume the weaker condition that

$$
\mathbb{E}\left|\frac{X^N_{11}-\hat\mu_N}{\hat\sigma_N}\right|^4=o(N^{2/3})
\quad\text{as }N\to\infty.
$$

It will also be evident that the argument can be adapted to more complicated exchangeability assumptions than the most basic one assumed above.

## 2. Proof of Theorem 1.1

Throughout the remainder of this article, we will use the notation $\partial_i f$ instead of the more familiar $\partial f/\partial x_i$. Similarly, we will write $\partial_i\partial_j f$ instead of $\partial^2f/(\partial x_i\partial x_j)$ and so on.

Now let us begin with the proof. Without loss of generality, we can assume that $X$ and $Y$ are defined on the same probability space and are independent. For each $i$, $0\le i\le n$, let

$$
Z_i=(X_1,\ldots,X_i,Y_{i+1},\ldots,Y_n)
\quad\text{and}\quad
Z_i^0=(X_1,\ldots,X_{i-1},0,Y_{i+1},\ldots,Y_n).
$$

Then clearly

$$
\mathbb{E}f(X)-\mathbb{E}f(Y)=\sum_{i=1}^n\left\{\mathbb{E}f(Z_i)-\mathbb{E}f(Z_{i-1})\right\}.
$$

Now, by third-order Taylor approximation,

$$
\left|f(Z_i)-f(Z_i^0)-X_i\partial_i f(Z_i^0)-\frac{X_i^2}{2}\partial_i^2f(Z_i^0)\right|
\le \frac{|X_i|^3L_3(f)}6
$$

and similarly,

$$
\left|f(Z_{i-1})-f(Z_i^0)-Y_i\partial_i f(Z_i^0)-\frac{Y_i^2}{2}\partial_i^2f(Z_i^0)\right|
\le \frac{|Y_i|^3L_3(f)}6.
$$

Now, since the $Y_i$'s are independent, we have

$$
\mathbb{E}\left((X_i-Y_i)\partial_i f(Z_i^0)\right)
=
\mathbb{E}\left(\left\{\mathbb{E}(X_i\mid X_1,\ldots,X_{i-1})-\mathbb{E}(Y_i)\right\}\partial_i f(Z_i^0)\right).
$$

Similarly, we also have

$$
\mathbb{E}\left((X_i^2-Y_i^2)\partial_i^2 f(Z_i^0)\right)
=
\mathbb{E}\left(\left\{\mathbb{E}(X_i^2\mid X_1,\ldots,X_{i-1})-\mathbb{E}(Y_i^2)\right\}\partial_i^2 f(Z_i^0)\right).
$$

Thus, for any $i$,

$$
\begin{aligned}
\left|\mathbb{E}f(Z_i)-\mathbb{E}f(Z_{i-1})\right|
&\le \frac16L_3(f)(\mathbb{E}|X_i|^3+\mathbb{E}|Y_i|^3) \\
&\quad+\left|\mathbb{E}\left((X_i-Y_i)\partial_i f(Z_i^0)\right)\right| \\
&\quad+\frac12\left|\mathbb{E}\left((X_i^2-Y_i^2)\partial_i^2 f(Z_i^0)\right)\right| \\
&\le \frac16L_3(f)M_3+A_iL_1(f)+\frac12B_iL_2(f).
\end{aligned}
$$

This completes the proof.

## 3. Proof of Theorem 1.2

First, note that $X=Y$ on the event $\{\hat\sigma=0\}$. Thus, if $\mathbb{P}\{\hat\sigma=0\}=1$, there is nothing to prove. If $\mathbb{P}\{\hat\sigma=0\}<1$, we can condition on the event $\{\hat\sigma>0\}$ and consequently assume, without loss of generality, that $\hat\sigma>0$ almost surely, because the conditioning retains the exchangeability of the $X_i$'s. Thus, let us assume that $\mathbb{P}\{\hat\sigma>0\}=1$.

For $i=1,\ldots,n$ let $\widetilde X_i=(X_i-\hat\mu)/\hat\sigma$. Then $\sum_{i=1}^n\widetilde X_i=0$ and $\sum_{i=1}^n\widetilde X_i^2=n$ (we will be using these identities numerous times, often without mention). Let $\widetilde Z_i=Z_i-\bar Z$, where $\bar Z=n^{-1}\sum_{i=1}^nZ_i$.

In the following, we will use $\mathbb{E}_0$ and $\mathbb{P}_0$ to denote the expectation and probability conditional on the pair $(\hat\mu,\hat\sigma)$. Observe that $\widetilde X$ is a vector with exchangeable components under $\mathbb{P}_0$ for all values of $(\hat\mu,\hat\sigma)$.

Now assume that $(\hat\mu,\hat\sigma)$ is given and fixed. Let

$$
f_0(x_1,\ldots,x_n):=f(\hat\mu+\hat\sigma x_1,\ldots,\hat\mu+\hat\sigma x_n).
$$

Then $f(X)=f_0(\widetilde X)$ and $f(Y)=f_0(\widetilde Z)$. Note that $L'_r(f_0)=L'_r(f)\hat\sigma^r$, where $L'_r(g)$ denotes a uniform bound on the $r$th order derivatives of a function $g$, including mixed partials.

First, we need to do a list of computations. For $0\le i\le n$, let $\mathcal F_i$ be the sigma-algebra generated by $\{\widetilde X_1,\ldots,\widetilde X_i\}$ and $(\hat\mu,\hat\sigma)$. Since the $\widetilde X_j$'s are exchangeable given $(\hat\mu,\hat\sigma)$, we have $\mathbb{E}_0(\widetilde X_k\mid\mathcal F_{i-1})=\mathbb{E}_0(\widetilde X_l\mid\mathcal F_{i-1})$ for every $k,l>i-1$, and hence

$$
\mathbb{E}_0(\widetilde X_i\mid\mathcal F_{i-1})
=
\mathbb{E}_0\left(\frac{1}{n-i+1}\sum_{j=i}^n\widetilde X_j\,\middle|\,\mathcal F_{i-1}\right).
$$

Now, since $\sum_{j=1}^n\widetilde X_j=0$,

$$
\frac{1}{n-i+1}\sum_{j=i}^n\widetilde X_j
=-\frac{1}{n-i+1}\sum_{j=1}^{i-1}\widetilde X_j,
$$

which is $\mathcal F_{i-1}$-measurable. Thus,

$$
\mathbb{E}_0(\widetilde X_i\mid\mathcal F_{i-1})
=-\frac{1}{n-i+1}\sum_{j=1}^{i-1}\widetilde X_j
=\frac{1}{n-i+1}\sum_{j=i}^n\widetilde X_j. \tag{3}
$$

From the above identity and exchangeability, it follows that

$$
\begin{aligned}
\mathbb{E}_0\left(\mathbb{E}_0(\widetilde X_i\mid\mathcal F_{i-1})^2\right)
&=\frac{1}{(n-i+1)^2}\Big[(n-i+1)\mathbb{E}_0(\widetilde X_1^2) \\
&\quad+(n-i+1)(n-i)\mathbb{E}_0(\widetilde X_1\widetilde X_2)\Big].
\end{aligned}
$$

Now clearly $\mathbb{E}_0(\widetilde X_1^2)=\mathbb{E}_0(n^{-1}\sum_{i=1}^n\widetilde X_i^2)=1$ and

$$
\begin{aligned}
\mathbb{E}_0(\widetilde X_1\widetilde X_2)
&=\frac{1}{n(n-1)}\sum_{i\ne j}\mathbb{E}_0(\widetilde X_i\widetilde X_j) \\
&=-\frac{1}{n(n-1)}\sum_{i=1}^n\mathbb{E}_0(\widetilde X_i^2)
=-\frac{1}{n-1}.
\end{aligned}
$$

(The second equality holds because $\sum_{j=1}^n\widetilde X_j=0$.) Combining, we get

$$
\mathbb{E}_0\left(\mathbb{E}_0(\widetilde X_i\mid\mathcal F_{i-1})^2\right)
=\frac{i-1}{(n-i+1)(n-1)}. \tag{4}
$$

Again, by a similar argument as before (using the identity $\sum_{i=1}^n\widetilde X_i^2=n$), we have

$$
\mathbb{E}_0(\widetilde X_i^2\mid\mathcal F_{i-1})
=\frac{1}{n-i+1}\sum_{j=i}^n\widetilde X_j^2.
$$

It follows that

$$
\begin{aligned}
\operatorname{Var}_0\left(\mathbb{E}_0(\widetilde X_i^2\mid\mathcal F_{i-1})\right)
&=\frac{1}{(n-i+1)^2}\Big[(n-i+1)\operatorname{Var}_0(\widetilde X_1^2) \\
&\quad+(n-i+1)(n-i)\operatorname{Cov}_0(\widetilde X_1^2,\widetilde X_2^2)\Big].
\end{aligned}
$$

Now, $\operatorname{Var}_0(\widetilde X_1^2)\le\mathbb{E}_0(\widetilde X_1^4)$, and

$$
\begin{aligned}
\operatorname{Cov}_0(\widetilde X_1^2,\widetilde X_2^2)
&=\frac{1}{n(n-1)}\sum_{i\ne j}\mathbb{E}_0(\widetilde X_i^2\widetilde X_j^2)
-\mathbb{E}_0(\widetilde X_1^2)\mathbb{E}_0(\widetilde X_2^2) \\
&=\frac{1}{n(n-1)}\sum_{i=1}^n\mathbb{E}_0\left(\widetilde X_i^2(n-\widetilde X_i^2)\right)-1 \\
&=\frac{1-\mathbb{E}_0(\widetilde X_1^4)}{n-1}\le0,
\end{aligned}
$$

since $\mathbb{E}_0(\widetilde X_1^4)\ge(\mathbb{E}_0(\widetilde X_1^2))^2=1$. Combining, we get

$$
\operatorname{Var}_0\left(\mathbb{E}_0(\widetilde X_i^2\mid\mathcal F_{i-1})\right)
\le \frac{\mathbb{E}_0(\widetilde X_1^4)}{n-i+1}. \tag{5}
$$

Now let $G$ be the matrix whose $(i,j)$th element is

$$
g_{ij}=\begin{cases}
1/(n-i+1), & i>j,\\
1, & i=j,\\
0, & i<j.
\end{cases}
$$

Let $R=G\widetilde X$. Then $R_i$ is $\mathcal F_i$-measurable, and from (3), we see that

$$
\mathbb{E}_0(R_i\mid\mathcal F_{i-1})=0. \tag{6}
$$

Next, note that

$$
\begin{aligned}
\mathbb{E}_0(R_i^2\mid\mathcal F_{i-1})
&=\mathbb{E}_0\left((\widetilde X_i-\mathbb{E}_0(\widetilde X_i\mid\mathcal F_{i-1}))^2\mid\mathcal F_{i-1}\right) \\
&=\mathbb{E}_0(\widetilde X_i^2\mid\mathcal F_{i-1})-\mathbb{E}_0(\widetilde X_i\mid\mathcal F_{i-1})^2.
\end{aligned}
$$

Using (4), (5), the triangle inequality and the fact that $\mathbb{E}_0(\widetilde X_i^2)=1$, we get

$$
\begin{aligned}
\mathbb{E}_0\left|\mathbb{E}_0(R_i^2\mid\mathcal F_{i-1})-1\right|
&\le \mathbb{E}_0\left|\mathbb{E}_0(\widetilde X_i^2\mid\mathcal F_{i-1})-1\right|
+\mathbb{E}_0\left(\mathbb{E}_0(\widetilde X_i\mid\mathcal F_{i-1})^2\right) \\
&\le \left(\frac{\mathbb{E}_0(\widetilde X_1^4)}{n-i+1}\right)^{1/2}
+\frac{i-1}{(n-i+1)(n-1)} \\
&\le 2\left(\frac{\mathbb{E}_0(\widetilde X_1^4)}{n-i+1}\right)^{1/2}
\end{aligned} \tag{7}
$$

since $\mathbb{E}_0(\widetilde X_1^4)\ge1$.

We will now temporarily use the notation $\|R_i\|_{3,0}$ for $(\mathbb{E}_0|R_i|^3)^{1/3}$, which is the conditional $L^3$ norm of $R_i$. By Minkowski's inequality and exchangeability, we have

$$
\|R_i\|_{3,0}
\le \|\widetilde X_i\|_{3,0}+\frac{1}{n-i+1}\sum_{j=1}^{i-1}\|\widetilde X_j\|_{3,0}
\le 2\|\widetilde X_1\|_{3,0}.
$$

This bound can be rewritten as

$$
\mathbb{E}_0|R_i|^3\le 8\hat\sigma^{-3}\mathbb{E}_0|X_1-\hat\mu|^3. \tag{8}
$$

Now define the function $f_1:\mathbb{R}^n\to\mathbb{R}$ as $f_1(x):=f_0(G^{-1}x)$. Then $f_1(R)=f_0(\widetilde X)$. Let $g_{ij}'$ denote the $(i,j)$th element of $G^{-1}$. It is a simple exercise to verify that

$$
g_{ij}'=\begin{cases}
-1/(n-j), & i>j,\\
1, & i=j,\\
0, & i<j.
\end{cases}
$$

Using the chain rule we see that for any $j$, $r$ and $x$,

$$
\partial_j^r f_1(x)
=\sum_{1\le i_1,\ldots,i_r\le n}(\partial_{i_1}\partial_{i_2}\cdots\partial_{i_r}f_0)(G^{-1}x)g'_{i_1j}g'_{i_2j}\cdots g'_{i_rj}.
$$

Thus for any $r$,

$$
L_r(f_1)\le L'_r(f_0)\max_{1\le j\le n}\left(\sum_{i=1}^n|g'_{ij}|\right)^r
= L'_r(f_0)2^r=L'_r(f)\hat\sigma^r2^r. \tag{9}
$$

Now let $V$ be a standard Gaussian vector in $\mathbb{R}^n$. Using the bounds from (6)--(9) in Theorem 1.1, we get

$$
\begin{aligned}
|\mathbb{E}_0 f_1(R)-\mathbb{E}_0 f_1(V)|
&\le \frac12L_2(f_1)\sum_{i=1}^n\mathbb{E}_0\left|\mathbb{E}_0(R_i^2\mid\mathcal F_{i-1})-1\right| \\
&\quad+\frac16 nL_3(f_1)\max_{1\le i\le n}(\mathbb{E}_0|R_i|^3+\mathbb{E}|V_i|^3) \\
&\le 4L'_2(f)\hat\sigma^2\sum_{i=1}^n\left(\frac{\mathbb{E}_0(\widetilde X_1^4)}{n-i+1}\right)^{1/2} \\
&\quad+\frac86 nL'_3(f)\hat\sigma^3\left(8\hat\sigma^{-3}\mathbb{E}_0|X_1-\hat\mu|^3+\mathbb{E}|V_1|^3\right).
\end{aligned}
$$

Now $\mathbb{E}|\widetilde X_1|^4=\hat\sigma^{-4}\mathbb{E}_0|X_1-\hat\mu|^4$, and by comparing sums with integrals, we have $\sum_{i=1}^n(n-i+1)^{-1/2}\le2\sqrt n$. Thus,

$$
\begin{aligned}
|\mathbb{E}_0 f_1(R)-\mathbb{E}_0 f_1(V)|
&\le 8L'_2(f)\sqrt{n\mathbb{E}_0|X_1-\hat\mu|^4} \\
&\quad+\frac43 nL'_3(f)\left(8\mathbb{E}_0|X_1-\hat\mu|^3+\hat\sigma^3\mathbb{E}|V_1|^3\right). \tag{10}
\end{aligned}
$$

Let $U=G^{-1}V$. Explicitly,

$$
U_i=V_i-\sum_{j=1}^{i-1}\frac{V_j}{n-j}.
$$

Now note that $f_1(V)=f_0(U)$, $f_0(\widetilde Z)=f(Y)$ and $f_1(R)=f_0(\widetilde X)=f(X)$. Combining, we get

$$
\begin{aligned}
|\mathbb{E}_0 f(X)-\mathbb{E}_0 f(Y)|
&=|\mathbb{E}_0 f_1(R)-\mathbb{E}_0 f_0(\widetilde Z)| \\
&\le |\mathbb{E}_0 f_1(R)-\mathbb{E}_0 f_1(V)|
+|\mathbb{E}_0 f_0(U)-\mathbb{E}_0 f_0(\widetilde Z)|. \tag{11}
\end{aligned}
$$

We already have a bound on $|\mathbb{E}_0f_1(R)-\mathbb{E}_0f_1(V)|$ from (10). We will now compute a bound on $|\mathbb{E}_0f_0(U)-\mathbb{E}_0f_0(\widetilde Z)|$, where recall that $\widetilde Z_i=Z_i-\bar Z$, and $Z$ is a standard Gaussian vector. To do that, we first need to do some computations. Let $\widetilde\sigma_{ij}:=\operatorname{Cov}(U_i,U_j)$. Then

$$
\widetilde\sigma_{ij}=\begin{cases}
-(n-j)^{-1}+\displaystyle\sum_{k=1}^{j-1}(n-k)^{-2}, & i>j,\\[1ex]
1+\displaystyle\sum_{k=1}^{j-1}(n-k)^{-2}, & i=j,\\[1ex]
\widetilde\sigma_{ji}, & i<j.
\end{cases}
$$

Now, for $i>j$, we can rewrite the first term in $\widetilde\sigma_{ij}$ as a telescoping sum to get

$$
\begin{aligned}
\widetilde\sigma_{ij}
&=-\frac{1}{n-1}-\sum_{k=1}^{j-1}\left(\frac{1}{n-k-1}-\frac{1}{n-k}\right)+\sum_{k=1}^{j-1}\frac{1}{(n-k)^2} \\
&=-\frac{1}{n-1}-\sum_{k=1}^{j-1}\frac{1}{(n-k)^2(n-k-1)}.
\end{aligned}
$$

Thus, if we define

$$
\sigma_{ij}:=\operatorname{Cov}(\widetilde Z_i,\widetilde Z_j)=
\begin{cases}
-1/n, & i\ne j,\\
(n-1)/n, & i=j,
\end{cases}
$$

then

$$
\begin{aligned}
\sum_{i,j}|\sigma_{ij}-\widetilde\sigma_{ij}|
&=\sum_{i=1}^n|\sigma_{ii}-\widetilde\sigma_{ii}|+2\sum_{i=1}^n\sum_{j=1}^{i-1}|\sigma_{ij}-\widetilde\sigma_{ij}| \\
&\le 2+\sum_{i=1}^n\sum_{k=1}^{i-1}\frac{1}{(n-k)^2}
+2\sum_{i=1}^n\sum_{j=1}^{i-1}\sum_{k=1}^{j-1}\frac{1}{(n-k)^2(n-k-1)} \\
&=2+\sum_{k=1}^{n-1}\frac{1}{n-k}+\sum_{k=1}^{n-2}\frac{1}{n-k} \\
&=3+2\sum_{k=2}^{n-1}\frac1k. \tag{12}
\end{aligned}
$$

We will use the well-known "Gaussian interpolation technique" for bounding $|\mathbb{E}_0f_0(U)-\mathbb{E}_0f_0(\widetilde Z)|$. This classical method for proving Slepian-type inequalities has been used extensively in recent years by Talagrand [19] in his efforts to obtain a rigorous version of the cavity method for spin glasses. For each $t\in[0,1]$, let $W_t=\sqrt{1-t}\,U+\sqrt t\,\widetilde Z$. Then

$$
\begin{aligned}
\mathbb{E}_0f_0(\widetilde Z)-\mathbb{E}_0f_0(U)
&=\mathbb{E}_0\left[\int_0^1\frac{d}{dt}f_0(W_t)\,dt\right] \\
&=\mathbb{E}_0\left[\int_0^1\sum_{i=1}^n\left(\frac{\widetilde Z_i}{2\sqrt t}-\frac{U_i}{2\sqrt{1-t}}\right)\partial_i f_0(W_t)\,dt\right]. \tag{13}
\end{aligned}
$$

Now, if a random vector $\xi=(\xi_1,\ldots,\xi_n)$ has a centered Gaussian distribution, then it is not difficult to show using integration by parts that for any differentiable function $h$ with subexponential growth at infinity, and any $i$, the following identity holds:

$$
\mathbb{E}(\xi_i h(\xi))=\sum_{j=1}^n\mathbb{E}(\xi_i\xi_j)\mathbb{E}(\partial_jh(\xi)).
$$

Since we do not want to expand our list of references, let us refer to Appendix A.6 of Talagrand's book [19] for a proof. Applying this result to our problem (after noting that interchanging integrals is not an issue since everything is bounded), we get

$$
\mathbb{E}_0(U_i\partial_i f_0(W_t))=\sqrt{1-t}\sum_{j=1}^n\widetilde\sigma_{ij}\mathbb{E}_0(\partial_j\partial_i f_0(W_t))
$$

and similarly,

$$
\mathbb{E}_0(\widetilde Z_i\partial_i f_0(W_t))=\sqrt t\sum_{j=1}^n\sigma_{ij}\mathbb{E}_0(\partial_j\partial_i f_0(W_t)).
$$

Combining, we have

$$
\mathbb{E}_0f_0(\widetilde Z)-\mathbb{E}_0f_0(U)
=\frac12\int_0^1\sum_{1\le i,j\le n}\mathbb{E}_0[\partial_i\partial_jf_0(W_t)](\sigma_{ij}-\widetilde\sigma_{ij})\,dt.
$$

Using the bound from (12), we get

$$
|\mathbb{E}_0f_0(U)-\mathbb{E}_0f_0(\widetilde Z)|
\le \frac12L'_2(f_0)\left(3+2\sum_{k=2}^{n-1}\frac1k\right). \tag{14}
$$

Combining this with (10) and (14), we get

$$
\begin{aligned}
|\mathbb{E}f(X)-\mathbb{E}f(Y)|
&\le \mathbb{E}|\mathbb{E}_0f(X)-\mathbb{E}_0f(Y)| \\
&\le 8L'_2(f)\sqrt{n\mathbb{E}|X_1-\hat\mu|^4} \\
&\quad+\frac43 nL'_3(f)\left(8\mathbb{E}|X_1-\hat\mu|^3+\mathbb{E}(\hat\sigma^3)\mathbb{E}|V_1|^3\right) \\
&\quad+\frac12L'_2(f)\mathbb{E}(\hat\sigma^2)\left(3+2\sum_{k=2}^{n-1}\frac1k\right).
\end{aligned}
$$

To complete the proof, we apply Jensen's inequality to get $\mathbb{E}(\hat\sigma^r)\le\mathbb{E}|X_1-\hat\mu|^r$ for $r\ge2$ and use the crude bounds $3+2\sum_{k=2}^{n-1}k^{-1}\le3\sqrt n$ and $\mathbb{E}|V_1|^3\le1.7$ to unify terms.

## 4. Proof of Theorem 1.3

We will now prove Theorem 1.3 via an application of Theorem 1.2, by using the Stieltjes transform of the spectral measure as a smooth function of the matrix entries. The Stieltjes transform (or Cauchy transform, or resolvent) of a cumulative probability distribution function $F$ on $\mathbb{R}$ is defined as

$$
m_F(z):=\int_{-\infty}^{\infty}\frac{1}{x-z}\,dF(x)\qquad\text{for every }z\in\mathbb{C}\setminus\mathbb{R}. \tag{15}
$$

Analogously, the Stieltjes transform of an $N\times N$ Hermitian matrix $A$ at a number $z\in\mathbb{C}\setminus\mathbb{R}$ is defined as

$$
m_A(z):=\frac1N\operatorname{Tr}\left((A-zI)^{-1}\right), \tag{16}
$$

where $I$ is the identity matrix of order $N$. Note that this is just the Stieltjes transform of the empirical spectral distribution (ESD) of $A$. The ESDs of a sequence $\{A_N\}_{N=1}^{\infty}$ of random Hermitian matrices converge weakly in probability to a distribution $F$ if and only if

$$
m_{A_N}(z)\xrightarrow{P}m_F(z)\qquad\text{for every }z\in\mathbb{C}\setminus\mathbb{R}.
$$

For the proof of this result and further details like Berry--Esseen-type error bounds, we refer to [2], pages 639--640.

Now recall that if $A(x)$ is a matrix-valued differentiable function of a scalar $x$, and $G(x):=(A(x)-zI)^{-1}$, where $z\in\mathbb{C}\setminus\mathbb{R}$ and $I$ is the identity matrix, then

$$
\frac{dG}{dx}=-G\frac{dA}{dx}G. \tag{17}
$$

This standard result is obtained by differentiating both sides of the identity $G(A-zI)\equiv I$. Differentiability follows from the fact that the elements of the inverse of a matrix are all rational functions of the elements of the original matrix. Higher-order derivatives may be computed by repeatedly applying the above formula.

The following lemma is the key to the proof of Theorem 1.3:

### Lemma 4.1

Suppose that for each $N$ we have a random matrix $\widetilde A_N=(N^{-1/2}\widetilde X^N_{ij})_{1\le i,j\le N}$, where the collection $(\widetilde X^N_{ij})_{1\le i\le j\le N}$ is exchangeable and $\widetilde X^N_{ij}=\widetilde X^N_{ji}$ for $i>j$. Suppose

$$
\frac{2}{N(N+1)}\sum_{i\le j\le N}\widetilde X^N_{ij}=0
\quad\text{and}\quad
\frac{2}{N(N+1)}\sum_{i\le j\le N}(\widetilde X^N_{ij})^2=1\quad\text{a.s.}
$$

For each $N$, let $(Z^N_{ij})_{1\le i\le j\le N}$ be a collection of i.i.d. standard Gaussian random variables and let $Y^N_{ij}=Z^N_{ij}-\bar Z^N$, where

$$
\bar Z^N=\frac{2}{N(N+1)}\sum_{i\le j}Z^N_{ij}.
$$

Let $Y^N_{ij}=Y^N_{ji}$ for $i>j$, and let $B_N=(N^{-1/2}Y^N_{ij})_{1\le i,j\le N}$. Then, for any $z\in\mathbb{C}\setminus\mathbb{R}$, and any $g:\mathbb{R}\to\mathbb{R}$ with bounded derivatives up to the third order, we have

$$
\left|\mathbb{E}g\left(\operatorname{Re}m_{\widetilde A_N}(z)\right)
-\mathbb{E}g\left(\operatorname{Re}m_{B_N}(z)\right)\right|
\le C_1N^{-1}\left(\mathbb{E}|\widetilde X^N_{12}|^4\right)^{1/2}
+C_2N^{-1/2}\mathbb{E}|\widetilde X^N_{12}|^3,
$$

where $m$ is the Stieltjes transform as defined in (16) and $C_1$ and $C_2$ are constants depending only on $g$ and $z$. The quantity

$$
\left|\mathbb{E}g\left(\operatorname{Im}m_{\widetilde A_N}(z)\right)
-\mathbb{E}g\left(\operatorname{Im}m_{B_N}(z)\right)\right|
$$

also admits the same upper bound.

To complete the proof of Theorem 1.3 using this lemma, we need the following fact about spectral distributions of Hermitian matrices:

### Lemma 4.2 (Quoted from [2], Lemma 2.2)

Let $A$ and $B$ be two $N\times N$ Hermitian matrices, with empirical distribution functions $F_A$ and $F_B$. Then

$$
\|F_A-F_B\|_\infty\le\frac1N\operatorname{rank}(A-B).
$$

This lemma is an easy consequence of the well-known interlacing inequalities for eigenvalues of Hermitian matrices. Let us now complete the proof of Theorem 1.3 by combining Lemma 4.1 and Lemma 4.2.

### Proof of Theorem 1.3

Let $\widetilde X^N_{ij}=(X^N_{ij}-\hat\mu_N)/\hat\sigma_N$, and let $\widetilde A_N=(N^{-1/2}\widetilde X^N_{ij})_{1\le i,j\le N}$. Clearly, $\widetilde A_N$ satisfies the hypotheses of Lemma 4.1. Thus, we have

$$
\left|\mathbb{E}g\left(\operatorname{Re}m_{\widetilde A_N}(z)\right)
-\mathbb{E}g\left(\operatorname{Re}m_{B_N}(z)\right)\right|
\le C_1N^{-1}\left(\mathbb{E}|\widetilde X^N_{12}|^4\right)^{1/2}
+C_2N^{-1/2}\mathbb{E}|\widetilde X^N_{12}|^3.
$$

The same bound holds for

$$
\left|\mathbb{E}g\left(\operatorname{Im}m_{\widetilde A_N}(z)\right)
-\mathbb{E}g\left(\operatorname{Im}m_{B_N}(z)\right)\right|
$$

as well. The bound converges to zero if $\mathbb{E}|\widetilde X^N_{12}|^4=o(N^{2/3})$, and thus under that condition, $\widetilde A_N$ and $B_N$ must have the same LSD. Finally, observe that by Lemma 4.2, the sequence $\{\hat\sigma_N^{-1}A_N\}$ has the same LSD as $\{\widetilde A_N\}$, and $F_{B_N}$ converges weakly to the semicircle distribution in probability. This completes the proof.

### Proof of Lemma 4.1

To formalize things in a way that is suitable for our purpose, consider the map $A$ which "constructs" Wigner matrices of order $N$. Let $n=N(N+1)/2$ and write elements of $\mathbb{R}^n$ as $x=(x_{ij})_{1\le i\le j\le N}$. For any $x\in\mathbb{R}^n$, let $A(x)$ be the matrix defined as

$$
A(x)_{ij}:=\begin{cases}
N^{-1/2}x_{ij}, & i\le j,\\
N^{-1/2}x_{ji}, & i>j.
\end{cases} \tag{18}
$$

Now let us fix $z=u+\sqrt{-1}v\in\mathbb{C}$, with $v\ne0$. Let $G(x):=(A(x)-zI)^{-1}$, and define $h:\mathbb{R}^n\to\mathbb{R}$ as

$$
h(x):=N^{-1}\operatorname{Tr}(G(x)).
$$

For any $\alpha\in\{(i,j)\}_{1\le i\le j\le N}$, we will write $\partial_\alpha h$ for $\partial h/\partial x_\alpha$ by our usual convention. From (17), it follows that for any $\alpha$,

$$
\partial_\alpha h=-N^{-1}\operatorname{Tr}(G(\partial_\alpha A)G). \tag{19}
$$

Now note that for any $\alpha,\beta\in\{(i,j)\}_{1\le i\le j\le N}$, we have $\partial_\beta\partial_\alpha A\equiv0$. An easy computation involving repeated applications of (17) to the above expression for $\partial_\alpha h$ gives, for any $\alpha,\beta,\gamma\in\{(i,j)\}_{1\le i\le j\le N}$,

$$
\partial_\beta\partial_\alpha h
=N^{-1}\sum_{\{\beta',\alpha'\}=\{\beta,\alpha\}}
\operatorname{Tr}(G(\partial_{\beta'}A)G(\partial_{\alpha'}A)G), \tag{20}
$$

$$
\partial_\gamma\partial_\beta\partial_\alpha h
=-N^{-1}\sum_{\{\gamma',\beta',\alpha'\}=\{\gamma,\beta,\alpha\}}
\operatorname{Tr}(G(\partial_{\gamma'}A)G(\partial_{\beta'}A)G(\partial_{\alpha'}A)G). \tag{21}
$$

Note that the first sum runs over all permutations of $(\beta,\alpha)$, which amounts to only two terms. Similarly, the second sum involves six terms.

To bound (19), first note that $\operatorname{Tr}(G(\partial_\alpha A)G)=\operatorname{Tr}((\partial_\alpha A)G^2)$. Since $G^2$ has a spectral decomposition and all its eigenvalues are bounded by $|v|^{-2}$ in magnitude, it follows in particular that the elements of $G^2$ are also bounded by $|v|^{-2}$. Now, $\partial_\alpha A$ has at most two nonzero elements, which are equal to $N^{-1/2}$. Hence,

$$
|\operatorname{Tr}(G(\partial_\alpha A)G)|=|\operatorname{Tr}((\partial_\alpha A)G^2)|\le2|v|^{-2}N^{-1/2}.
$$

To bound (20) and (21), we need to recall the properties of the Hilbert--Schmidt norm for matrices. For an $N\times N$ complex matrix $B=(b_{ij})_{1\le i,j\le N}$, the Hilbert--Schmidt norm of $B$ is defined as $\|B\|=(\sum_{i,j}|b_{ij}|^2)^{1/2}$. Besides the usual properties of a matrix norm, it has the following additional features: (a) $|\operatorname{Tr}(BC)|\le\|B\|\|C\|$, (b) if $U$ is a unitary matrix, then for any $C$ of the same order, $\|CU\|=\|UC\|=\|C\|$, and (c) for a matrix $B$ admitting a spectral decomposition (i.e., a normal matrix) with eigenvalues $\lambda_1,\ldots,\lambda_N$, and any other matrix $C$ of the same order, $\max\{\|BC\|,\|CB\|\}\le\max_{1\le i\le N}|\lambda_i|\cdot\|C\|$. For a proof of these standard facts one can look up, for example, [22], pages 55--58.

Clearly, $G$ and the derivatives of $A$ are all normal matrices. Moreover, the eigenvalues of $G$ are bounded by $|v|^{-1}$, where $v=\operatorname{Im}z$. Thus, by the properties of the Hilbert--Schmidt norm listed above, we have

$$
\begin{aligned}
|\operatorname{Tr}(G(\partial_\beta A)G(\partial_\alpha A)G)|
&\le \|G(\partial_\beta A)\|\,\|G(\partial_\alpha A)G\| \\
&\le |v|^{-3}\|\partial_\beta A\|\,\|\partial_\alpha A\| \\
&\le 2|v|^{-3}N^{-1}.
\end{aligned}
$$

Similarly,

$$
\begin{aligned}
|\operatorname{Tr}(G(\partial_\gamma A)G(\partial_\beta A)G(\partial_\alpha A)G)|
&\le \|G(\partial_\gamma A)\|\,\|G(\partial_\beta A)G(\partial_\alpha A)G\| \\
&\le \|G(\partial_\gamma A)\|\,\|G(\partial_\beta A)G\|\,\|(\partial_\alpha A)G\| \\
&\le |v|^{-4}\|\partial_\gamma A\|\,\|\partial_\beta A\|\,\|\partial_\alpha A\| \\
&\le 2^{3/2}|v|^{-4}N^{-3/2}.
\end{aligned}
$$

Finally, note that since the matrix entries are all real, therefore $\partial_\alpha(\operatorname{Re}h)=\operatorname{Re}\partial_\alpha h$ and so on. Thus, if we let $f=g\circ(\operatorname{Re}h)$, then substituting the bounds obtained above in (19), (20) and (21), we get $L'_2(f)\le K_1N^{-2}$ and $L'_3(f)\le K_2N^{-5/2}$, where $K_1$ and $K_2$ are constants depending only on $g$ and $z$. By Theorem 1.2, it now follows that

$$
|\mathbb{E}f(\widetilde X)-\mathbb{E}f(Y)|
\le 9.5K_1N^{-1}\left(\mathbb{E}|\widetilde X_{12}|^4\right)^{1/2}
+13K_2N^{-1/2}\mathbb{E}|\widetilde X_{12}|^3,
$$

where $Y_{ij}=Z_{ij}-\bar Z$, and $Z_{ij}$'s are i.i.d. standard Gaussian random variables. This completes the proof of the lemma.

## Acknowledgments

The author thanks the anonymous referee for his very detailed and helpful comments on the material and the style of presentation. He is also grateful to his former thesis advisor Persi Diaconis for constant encouragement and support.

## References

[1] Arnold, L. (1967). On the asymptotic distribution of the eigenvalues of random matrices. *J. Math. Anal. Appl.* **20** 262--268. MR0217833

[2] Bai, Z. D. (1999). Methodologies in the spectral analysis of large-dimensional random matrices, a review. *Statist. Sinica* **9** 611--677. MR1711663

[3] Baik, J. and Suidan, T. M. (2005). A GUE central limit theorem and universality of directed first and last passage site percolation. *Int. Math. Res. Not.* **6** 325--337. MR2131383

[4] Bodineau, T. and Martin, J. (2005). A universality property for last-passage percolation paths close to the axis. *Electron. Comm. Probab.* **10** 105--112. MR2150699

[5] Chatterjee, S. (2004). A simple invariance theorem. Available at `http://arxiv.org/math.PR/0508213`.

[6] De Finetti, B. (1969). Sulla prosequibilità di processi aleatori scambiabili. *Rend. Ist. Mat. Univ. Trieste* **1** 53--67. MR0292146

[7] Boutet de Monvel, A. and Khorunzhy, A. (1998). Limit theorems for random matrices. *Markov Process. Related Fields* **4** 175--197. MR1641617

[8] Diaconis, P. and Freedman, D. (1980). Finite exchangeable sequences. *Ann. Probab.* **8** 745--764. MR0577313

[9] Girko, V. L. (1988). *Spectral Theory of Random Matrices*. Nauka, Moscow. MR0955497

[10] Grenander, U. (1963). *Probabilities on Algebraic Structures*. Wiley, New York. MR0259969

[11] Khorunzhy, A. M., Khoruzhenko, B. A. and Pastur, L. A. (1996). Asymptotic properties of large random matrices with independent entries. *J. Math. Phys.* **37** 5033--5060. MR1411619

[12] Lindeberg, J. W. (1922). Eine neue herleitung des exponentialgesetzes in der wahrscheinlichkeitsrechnung. *Math. Z.* **15** 211--225. MR1544569

[13] Mossel, E., O'Donnell, R. and Oleszkiewicz, K. (2005). Noise stability of functions with low influences: Invariance and optimality. Available at `http://arxiv.org/math.PR/0503503`.

[14] Pastur, L. A. (1972). The spectrum of random matrices. *Teoret. Mat. Fiz.* **10** 102--112. MR0475502

[15] Paulauskas, V. and Račkauskas, A. (1989). *Approximation Theory in the Central Limit Theorem. Exact Results in Banach Spaces*. Kluwer, Dordrecht. MR1015294

[16] Rotar, V. I. (1979). Limit theorems for polylinear forms. *J. Multivariate Anal.* **9** 511--530. MR0556909

[17] Schenker, J. H. and Schulz-Baldes, H. (2005). Semicircle law and freeness for random matrices with symmetries or correlations. *Math. Res. Lett.* **12** 531--542. MR2155229

[18] Suidan, T. (2006). A remark on a theorem of Chatterjee and last passage percolation. *J. Phys. A* **39** 8977--8981. MR2240468

[19] Talagrand, M. (2003). *Spin Glasses: A Challenge for Mathematicians. Cavity and Mean Field Models*. Springer, Berlin. MR1993891

[20] Trotter, H. F. (1959). Elementary proof of the central limit theorem. *Archiv der Mathem.* **10** 226--234. MR0108847

[21] Wigner, E. P. (1958). On the distribution of the roots of certain symmetric matrices. *Ann. of Math.* (2) **67** 325--327. MR0095527

[22] Wilkinson, J. H. (1965). *The Algebraic Eigenvalue Problem*. Clarendon Press, Oxford. MR0184422

[23] Zolotarev, V. M. (1977). Ideal metrics in the problem of approximating the distributions of sums of independent random variables. *Theory Probab. Appl.* **22** 449--465. MR0455066

---

Department of Statistics  
367 Evans Hall #3860  
University of California, Berkeley  
Berkeley, California 94720  
USA  
Email: `sourav@stat.berkeley.edu`  
URL: `http://www.stat.berkeley.edu/~sourav`
