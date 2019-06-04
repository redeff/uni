## Ejercico de ejemplo

Para seno en x = 0,
$$ P_3(x) = f(0) + xf'(0) + x^2\frac{f''(0)}{2!} + x^3\frac{f'''(0)}{3!} $$
$$ P_3(x) = x - \frac{x^3}{3!} $$

## Ejercicio de Ejemplo

Hallar los polinomios de taylor de orden k entre 0 y 5 de $\lambda x \to \sin x$
desarrollados en $x_0 = 0$

$$P_0(x) = 0$$
$$P_1(x) = x$$
$$P_2(x) = x$$
$$P_3(x) = x - \frac{x^3}{3!}$$
$$P_3(x) = x - \frac{x^3}{3!}$$
$$P_5(x) = x - \frac{x^3}{3!} + \frac{x^5}{5!}$$

## Ejercicio de Ejemplo

Calcular el valor de $3 \ln 2$ en forma aproximada usando el Polinomio de
Taylor de orden 3 evaluado en algún $x_1$

Usando la funcion:

$f(x) = 3 \ln (1 + 2x)$

Queremos evaluarla en \frac{1}{2}, y nos gusta centrarla en x = 0

$f(x) = 3 ln (1 + 2x) => f(0) = 0$

$f'(x) = \frac{6}{1 + 2x} => f'(0) =>  6$

$f''(x) = -12(1 + 2x)^{-2} => f''(0) => -12$

$f'''(x) = 48(1 + 2x)^{-3} => f'''(0) => 48$

$f''''(x) = -228(1 + 2x)^{-4} => f''''(0) = -288$

Ahora calcularmos el polinomio

$P_3(x) = f(0) + f'(0) + \frac{f''(0)}{2} + \frac{f'''(0)}{3}$

$P_3(x) = 0 + 6x - \frac{12x^2}{2} + \frac{48x^3}{6}$

$P_3(x) = 6x - 6x^2 + 16x^3$

Evaluamos en $\frac{1}{2}$ tenemos:

$$P_3\left(\frac{1}{2}\right) = \frac{6}{2} + 16 \times \left(\frac{1}{2}\right) = 2.5$$


# Ejercicios: dados dos taylors sacar taylors del producto o cociente
## Ejercicio 7

Los taylor de orden 4 de $f$ y $g$ en $x = 2$ son

$$p(x) = -2+3(x-2)-3(x-2)^2+(x-2)^3$$
$$q(x) = 5+12(x-2)^2-7(x-2)^4$$

Hallar el taylor de orden 2 de:

$$t(x) = f(x)g(x)$$
$$s(x) = \frac{f(x)}{g(x)}$$

Para hallar el taylor 2 necesitamos $t(2)$, $t'(2)$ y $t''(2)$

Calculemos las derivadas de $f$ y $g$ en 2

$$f(2) = p(2) = -2$$

$$f'(2) = p'(2) = 3$$

$$f''(2) = p''(2) = (-3)(2!) = -6$$

$$f'''(2) = p'''(2) = (1)(3!) = 6$$

$$f^{IV}(2) = p'''(2) = (0)(4!) = 0$$

Las derivadas de $t$ son:
$$t(x) = f(x)g(x)$$

$$t'(x) = f'(x)g(x) + f(x)g'(x)$$

$$t''(x) = f''(x)g(x) + 2f'(x)g'(x) + f(x)g''(x)$$

Queda como el binomio de Newton en gral

Ahí evaluamos las derivadas y construimos el poly de taylor.
Queda

$t(x) = -10 + 15(x-2) - 39(x-2)^2$

## Ejercicio 11 Varios
tenemos $g(x) = 1 - 3x + \sqrt{f(x)}$
Y tenemos el poly de taylor de orden 2 de $g$.

Queremos calcular el poly de taylor de orden 2 de $f$
Derivo la ecuación que tengo y igualo las derivadas de $g$ con las de el
poly de taylor de $g$, así despejo las derivadas de $f$

## Ejercicio 8

Sea $f(x) = \ln(1+x)$
Hacemos los polinomios de taylor

Usamos la fŕomula del resto y tenemos:

$$R_3(x) = -\frac{6}{24}\frac{1}{(1+c)^4}x^4$$

$$0 \le c \le x$$

$$1 \le c \le 1+x$$

$$1^4 \le c^4 \le (1+x)^4$$

Entonces el error se puede acotar con $1 \le c$:

$$|R_3(x)| \le \frac{6}{24}x^4$$

$$|R_3(x)| \le \frac{1}{4}x^4$$
