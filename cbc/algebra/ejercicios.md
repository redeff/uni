## Ejercicio 2019-06-04

Sean $S = \langle(2,1,3,3)\rangle$, $T=\{x\in R^4 \mid x_1-2x_2+x_3-x_4=0\}$

Definir, si es posible, $f : R^4 \to R^4$, tal que:

$Nuf \bigoplus S = T$

$Nu(f\circ f) = T$

## Ejercicio 2019-06-05

$f : R^3 \to R^3$

$B = \{(1, 1, 1) (0, 1, -1), (0, 0 -1)\}$

$B' = \{(1, -1, 0) (0, 0, 1), v\}$

$M_{BB'}f = \begin{bmatrix}1 & 0 & 2 \\ 1 &2 &0 \\ 1 & -1 & 1\end{bmatrix}$

a) Hallar $v \in R^3$ para $f(0, 0, 1) = (-2, 3, 2)$

b) Si $S = \langle(-1, 1, 0)\rangle$ hallar una base de $fS$

c) Decidir si $f$ es *iso*

<!-- comment -->

a) Tenemos $(f(0, 0, 1))_{B^'} = M_{BB'}f \cdot (0, 0, 1)_{B} = M_{BB'}f \cdot (0, 0, -1) =$

  $=\begin{bmatrix}1 & 0 & 2 \\ 1 &2 &0 \\ 1 & -1 & 1\end{bmatrix} \cdot (0, 0,
 -1) = (-2, 0, -1)$

 $(-2, 3, 2)_{B^'} = (f(0, 0, -1))_{B^'} = (-2, 0, -1)$

 $(-2, 3, 2) = -2(1, -1, 0) - v$

 $v = -2(1, -1, 0) - (-2, 3, 2)$

 $v = (0, -1, -2)$

b) Hay que calcular $f(-1, 1, 0)$. Tenemos:

 $(f(-1, 1, 0))_{B'} = M_{BB^'} \cdot (-1, 1, 0)_B$

 Resolvemos el sist $\left[\begin{smallmatrix}
 1 & 0 & 0\\
 1 & 1 & 0\\
 -1 & -1 & 0
 \end{smallmatrix} \;\middle|\;
 \begin{smallmatrix}
 -1 \\
 1 \\
 -1
 \end{smallmatrix}\right]$, queda $(-1, 1, 0)_{B} = (1, 2, 3)$

 Reemplazamos $(f(-1, 1, 0))_{B^'} = \begin{bmatrix}1 & 0 & 2 \\ 1 &2 &0 \\ 1 & -1 & 1\end{bmatrix} \cdot (1, 2, 3) = (-7, 3, -6)$

 Entonces $f(-1, 1, 0) = -7(1, -1, 0) + 3(0, 0, 1) - 6(0, -1, 2)
 = (-7, 13,
 -9)$

 c) Como el rango de $M_{BB'}f$ es $3$, sabemos que $f$ es *iso*

# Cambio de base
Sean $B = \{(1 \; -1), (0 \; 2)\}$, $B^' = \{(2 \; 0), (-1 \; 3)\}$

Hallar $C_{BB^'}$, $C_{BE}$, $C_{EB}$

$C_{BB^'} = \left[
\begin{pmatrix}
1 \\
-1
\end{pmatrix}_{B^'}
\begin{pmatrix}
0 \\
2
\end{pmatrix}_{B^'}
\right] =$
$\begin{pmatrix}
\frac{1}{3} & \frac{1}{2}\\
-\frac{1}{3} & \frac{2}{3}
\end{pmatrix}$

$C_{BE}$ es fácil

$C_{EB}$ es la inversa de el anterior

## ejercicio

Sean $B = \{v_1 \; v_2 \; v_3\}$,

$B^'=\{v_1+v_2+v_3, v_2+v_3, v_3\}$, y

$B^{''} = \{v_1, v_1 - v_2, v_1 + v_2 - v_3\}$ Bases de $V$

Hallar $C_{B^'B}$, $C_{B^'B^{''}}$ y $C_{BB^'}$

$C_{B^'B}$ es $\begin{bmatrix}
1 & 0 & 0 \\
1 & 1 & 0 \\
1 & 1 & 1
\end{bmatrix}$

$C_{BB^'}$ es la inversa de la anterior

Para hacer $C_{B^'B^{''}}$ tenemos que hacer la cuenta:

$C_{B^'B^{''}} =
\left[
(B_1)_{B^{''}}
(B_2)_{B^{''}}
(B_3)_{B^{''}}
\right] =
\begin{bmatrix}
4 & 3 & 2\\
-2 & -5 & -1\\
-1 & -1 & -1\\
\end{bmatrix}$

# ejercicio

Sea $f : R^2 \to R^2 \mid f (x \; y) = (x-y, x+y)$,
$B = \{(1 \; -1), (1 \; 2)\}$

a) Probar $f$ *iso*

b) Hallar
	* $M_{BE} \; f$,
	* $M \; f^{-1}$,
	* $M_{BE}\; (f \circ f)$
