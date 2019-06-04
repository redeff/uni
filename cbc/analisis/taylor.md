# Def Polinomio de taylor

Sea $f:R\to R$, $n$ veces derivable en $x_0$. Se define el polinomo de Taylor de
$f(x)$ de orden $n$ desarrollado en $x = x_0$ a lo siguiente:

$$P_n(f(x), x_0 = x, x) = \sum_{k=0}^{k \leq n} f^{(k)}(x_0) \frac{(x - x_0)^k}{k!}$$

El valor que no está multiplicado por $(x-x_0)$ se lo llama "coeficiente
independiente"

#### Nota:

$0! = 1$

## Prop: Las primeras n derivadas coinciden

* $P_n(x_0) = f(x_0)$
* $P_n'(x_0) = f'(x_0)$, ...
* $P_n^{(n)}(x_0) = f^{(n)}(x_0)$

Osea todas las (primeras n) derivadas coinciden

## Prop

el grado del polinomio de Taylor de orden n es la lo sumo n

## Pasar polinomios de base

Si se tiene $P(x) = \sum a_ix^i$
Y se quiere hallar $b_i$ tal que $P(x) = \sum b_i (x - x_0)^i$,
hay que expandir los $(x - x_0)^i$ y queda un sist de ecuaciones

**o** se le puede hacer el polinomio de Taylor de orden $n$ al polinomio $P(x)$
en el punto $x=x_0$ (como es Poly, da exacto), que es más
fácil

## Prop

* **Derivación** La derivada del Poly de Taylor de orden n de f es el Poly
  de Taylor de orden n-1 de f'

  Osea $(P_{n,f})' = P_{n-1, f'}$

* **Linearidad:** $P_{f + g} = P_f + P_g, y P_{kf} = fP_f$

* **Sustitución:**

  $P(f(x), x_0, x) = P(f(cx), cx_0, x)$, y

  $P(f(x), x_0, x) = P(f(cx + k), x_0 + k, x)$, y en gral

  $P(f(x), x_0, x) = P(f(Q(x)), Q(x_0), x)$ , para todo poly $Q$

# Sacar taylor dado el taylor de una función relacionada

Si se tiene el polinomio de taylor $P_n$ de una función $f$ en $x_0$, y se
quere hallar el polinomio de taylor de $g$ y se sabe:

$g = h \circ f$, entonces sabemos:

$gx = h (fx)$

$g'x = h' (fx) \cdot f'x$

$g''x = h'' (fx) \cdot (f'x)^2 + h'(fx)\cdot f''x$, $...$

Así podemos evaluar las derivadas de $g$ en $x_0$ (ya que sabemos las
derivadas de $f$ en $x_0$), y entonces podemos computar el poly de taylor

# Sacar el taylor de un producto
Tenemos los taylors $P_n$ y $Q_n$ de $f$ y de $g$ y queremos hallar el poly
de taylor $R_n$ de $h(x) = f(x)\cdot g(x)$

Tenemos:

$h(x) = f(x)g(x)$

$h'(x) = f'(x)g(x) + f(x)g'(x)$

$h''(x) = f''(x)g(x) + 2f'(x)g'(x) + f(x)g''(x)$, $\dots$

Termina quedando como el binomio de Newton. Ahí podemos evaluar en $x_0$ y
sacar todas las derivadas
