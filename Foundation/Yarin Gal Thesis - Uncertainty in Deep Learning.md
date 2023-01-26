
#H1 Chapter 1

#H2: Deep Learning
Linear regression problem:
- $N$ Input output paris of data $\{(x_1, y_1),...(x_N, y_N)\}$
- Asume there exists a linear function that maps $x$ to $y$
- Model: $f(x) = Wx + b# Basically a linear transformation
	- $W \in R^{Q\times D}, b\in R^{D}$
	- Different parameters $W, b$ define different linear transformation
- Finding parameters that minimies the averaged MSE
	- $\frac{1}{N} \sum_{i} ||y_i - (x_i W + b)||^2$
---
- General cases: relation between $x$ and $y$ is not linear
	- resort to linear basis function regression
		- Basically, transform x using non-linear transformation $\phi$ to get feature vector
		- $\Phi(x)  = [\phi_1(x), ..., \phi_K(x)]$
		- Perform linear regression with this vector instead of the $x$
		- $\phi()$ are the basis functions, may be parameterized

---
	**Basis are orthogonal, sought out to be optimal. Orthogonality with polynomial basis exspansion?**
---

- Relax the constraint to be fixed and mutually orthogonal, use parameterized basis functions: Basis: $\phi_k^{w_k, b_k}$. 
	- Linear regression model: $f(x) = \Phi^{W_1, b_1}(x) W_2 + b_2$, $\Phi^{W_1, b_1} = \phi(W_1 x + b_1)
	- Deep learning models: hierarchy of such parameterized basis functions[]
	- 
---


