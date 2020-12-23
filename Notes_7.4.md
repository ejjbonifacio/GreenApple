### Systems of Linear Differential Equations

***

A system of $n$ first order linear equations can be written as:
$$
\begin{equation}
x_1' = p_{11}(t)x_1 + \dots + p_{1n}(t)x_n + g_1(t),\\
\vdots\\
x_n' = p_{n1}(t)x_1 + \dots + p_{nn}(t)x_n + g_n(t)
\end{equation}
$$
This can be converted to the following form:
$$
\mathbf{x}' = \mathbf{P}(t)\mathbf{x} + \mathbf{g}(t)
$$
The vector $ \mathbf{x} $ is a solution of this equation which is composed of functions $\phi_1(t) \dots \phi_n(t)$. A homogenous equation refers to systems with $\mathbf{g}(t) = 0$. We use the notation to designate specific solutions:
$$
\mathbf{x}^{(1)}(t) = 
\begin{bmatrix}
x_{11}(t)\\
\vdots\\
x_{n1}(t)
\end{bmatrix}, \dots,
\mathbf{x}^{(k)}(t) = 
\begin{bmatrix}
x_{1k}(t)\\
\vdots\\
x_{nk}(t)
\end{bmatrix}
$$

***

**Principle of Superposition**
If the vector functions $\mathbf{x}^{(1)}$ and $\mathbf{x}^{(2)}$ are the solutions of $\mathbf{x}' = \mathbf{P}(t) \mathbf{x}$, then the linear combinations $c_1 \mathbf{x^{(1)}} + c_2 \mathbf{x^{(2)}}$ is also a solution for any constants $c_1$ and $c_2$

***

**Wronskian**
For a system of $n$ first order equations, it is sufficient to form linear combinations of $n$ properly chosen solutions. Consider the matrix $\mathbf{X}(t)$ whose columns are $\mathbf{x}^{(1)} \dots \mathbf{x}^{(n)}$. The *Wronskian* is defined as:
$$
W[\mathbf{x}^{(1)}, \dots, \mathbf{x}^{(n)}](t) = \det \mathbf{X}(t)
$$
> The solutions $\mathbf{x}^{(1)} \dots \mathbf{x}^{(n)}$ are linearly independent at a point is and only if the Wronskian is not zero.

***

**Theorem 7.4.2**
If the vector functions $\mathbf{x}^{(1)}, \dots, \mathbf{x}^{(n)}$ are linearly independent solutions of $\mathbf{x}' = \mathbf{P}(t) \mathbf{x}$ for each point in the interval $\alpha < t < \beta$, then each solution $\mathbf{x} = \boldsymbol{\phi}(t)$ of the system can be expressed as  a linear combination of $\mathbf{x}^{(1)}, \dots, \mathbf{x}^{(n)}$ in exactly one way.

> The **general solution** of a system is $\boldsymbol{\phi}(t) = c_1\mathbf{x}^{(1)}(t) + \dots + c_n \mathbf{x}^{(n)}(t)$. The set of solutions $\mathbf{x}^{(1)}, \dots, \mathbf{x}^{(n)}$ that is linearly independent on the interval $\alpha < t < \beta$ is called the **fundamental set of solutions**. 

***

**Theorem 7.4.3**
If $\mathbf{x}^{(1)}, \dots, \mathbf{x}^{(n)}$ are the solutions of $\mathbf{x}' = \mathbf{P}(t) \mathbf{x}$ on the interval $\alpha < t < \beta$, then in this interval $W[\mathbf{x}^{(1)}, \dots, \mathbf{x}^{(n)}]$ either is identically zero or else never vanishes.

***

**Theorem 7.4.4**
Let
$$
\begin{aligned}
\mathbf{e}^{(1)} = 
\begin{bmatrix}
1\\0\\0\\ \vdots\\0
\end{bmatrix},
\mathbf{e}^{(2)} = 
\begin{bmatrix}
0\\1\\0\\ \vdots\\0
\end{bmatrix}, \dots,
\mathbf{e}^{(n)} = 
\begin{bmatrix}
0\\0\\0\\ \vdots\\1
\end{bmatrix}
\end{aligned}
$$
Let $\mathbf{x}^{(1)}, \dots, \mathbf{x}^{(n)}$ be the solutions of $\mathbf{x}' = \mathbf{P}(t) \mathbf{x}$ that satisfy the initial conditions
$$
\mathbf{x}^{(1)}(t_0) = \mathbf{e}^{(1)}, \dots, \mathbf{x}^{(n)}(t_0) = \mathbf{e}^{(n)},
$$
respectively, where $t_0$ is any point in $\alpha < t < \beta$. Then $\mathbf{x}^{(1)}, \dots, \mathbf{x}^{(n)}$ form a fundamental set of solutions of the system.

> In other words, the system has at least one fundamental set of solutions.