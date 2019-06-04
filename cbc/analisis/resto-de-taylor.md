# Resto de Taylor

$$R_n(x) = f(x) - P_n(x)$$

Se denomina el **resto** o **error** de Taylor. Queremos encontrar cotas
para $R_n$

Sabemos que las primeras $0\dots n$ derivadas de $R_n$ evaluadas en $0$ son $0$.
Tomemos el cociente:

$$\frac{R_n(x)}{x^{n+1}}=$$

$$\frac{R_n(x) - R_n(0)}{x^{n+1} - 0^{n+1}}=$$

$$\frac{R_n'(\xi)}{(n+1)\xi^{n}}$$

Por Cauchy con $f = R_n$ y $g(x) = x ^ {n+1}$,
para algún $\xi$ con $\xi$ entre 0 y x

Hacemos esto $n$ veces, y tenemos que:

$$\frac{R_n(x)}{x^{n+1}} = \frac{R_n^{(n+1)}(c)}{(n+1)!c^0}$$

Para algún $c$ entre $0$ y $x$, osea

$$R_n(x) = x^{n+1}\frac{R_n^{(n+1)}(c)}{(n+1)!}$$

$$R_n(x) = f^{(n+1)}(c)\frac{x^{n+1}}{(n+1)!}$$

Ya que la derivada $n+1$ de $f$ coincide con la de $R_n$

## En general tenemos

Si $f$ tiene $n+1$ derivadas continuas en $x_0$, luego

$$R_n(x) = \frac{f^{(n+1)}(c)}{(n+1)!}(x - x_0)^{n+1}$$

Para algún $c$ entre $x_0$ y $x$
