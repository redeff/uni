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

## Ejercicio 2019-06-07

Sean $B = \{(1, 1, 1); (0, 1, -1); (0, 0, -1)\}$,
$B' = \{(-1, 1, ); (0, 0, 1); (1, 2, 0)\}$

Si $M_{BB^'} = \begin{bmatrix}
1 & 0 & 2 \\
1 & 2 & 0 \\
1 & -1 & 1
\end{bmatrix}$

Hallar $M_{B'} \; (f \circ f)$

$M_{B^'} \; f = C_{B^'B^'} \cdot M_{BB^'} f \cdot C_{B^'B} \cdot M_{BB^'} f \cdot C_{B^'B}$

Encontrar $C_{B^'B}$ es resolver el sistema dado por $\left[C_{BE} \mid C_{B^'E}\right]$, osea

$\left[\begin{smallmatrix}
1 & 0 & 0 \\
1 & 1 & 0 \\
1 & -1 & -1
\end{smallmatrix} \;\middle|\;
\begin{smallmatrix}
-1 & 0 & 1 \\
1 & 0 & 2 \\
0 & 1 & 0 \\
\end{smallmatrix}\right] \to$
$\left[\begin{smallmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & -1 & -1
\end{smallmatrix} \;\middle|\;
\begin{smallmatrix}
-1 & 0 & 1 \\
2 & 0 & 1 \\
0 & 1 & -1 \\
\end{smallmatrix}\right] \to$
$\left[\begin{smallmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{smallmatrix} \;\middle|\;
\begin{smallmatrix}
-1 & 0 & 1 \\
2 & 0 & 1 \\
-3 & -1 & 0 \\
\end{smallmatrix}\right] =$

$\left[I \mid C_{B^'B}\right]$

También podemos hacer $C_{B^'B} = C_{EB} \cdot C_{B^'E}
= (C_{BE})^{-1} \cdot C_{B^'E}$

Sabemos que $C_{EX} = \left[X_i \mid \dots \right]$ para toda base $X$,
entonces son fáciles de calcular

También sabemos:
$M_{B^'} \; f = M_{BB^'} f \cdot C_{B^'B} \cdot M_{BB^'} f \cdot C_{B^'B} =$

$M_{B^'} \; f = (M_{BB^'} f \cdot C_{B^'B}) \cdot (M_{BB^'} f \cdot C_{B^'B}) =$

$M_{B^'} \; f = M_{B^'} f \cdot M_{B^'} f$

## ejercicio
$B = \{(1, 0, 1), (0, -1, 1), (-1, 0, 1)\}$

$f : R^3 \to R^3$

$M_{BE}f = \begin{bmatrix}
-2 & 1 & 0 \\
-5 & 1 & k \\
-8 & k & 2
\end{bmatrix}$

Hallar $f \in R \mid Nu \; f \neq \{0\}$, y además $Nu \; f \subseteq Im \; f$

Sabemos $Nu \; f \neq {0} \iff dim \; Im f \neq 3 \iff det \; M_{BE}f = 0$

$|M_{BE}| = 0 \iff k = 1$ ó $k = 3$, hay que ver cuándo se cuple la segunda
condición

Sabemos $Im f = \langle(-2, -5, -8)\; (1, 1, k)\; (0, k, 2)\rangle$

Para hallar el núcleo podemos hallar las soluciones de $\left[M_{BE}\mid\bar0\right]$, y esos vectores multiplicarlos por $C_{BE}$ para pasarlos a la canónica y compararlos con $Im \; f$


## Ejercicio 2
Sea $f : R^4 \to R^3$ TL, tal que $mf = \begin{bmatrix}
1 & 1 & -1 & 0 \\
0 & 1 & 3 & 0 \\
1 & 2 & 2 & 1
\end{bmatrix}$

a. $S = \langle(1,0,1,0);(-1,2,0,0)\rangle$ Hallar una base de $fS$

    $fS = \langle fS_1 ; fS_2\rangle$

b. Hallar $Imf$

    Necesitamos $\langle fB_1 \dots fB_n\rangle$, pero estos generadores son
    las columnas de $mf$

    Para hallar una base de $Imf$ tenemos que ver si las columnas son LI, es
    decir escalonamos $(mf)^T$

    En particular $Dim (Im f) = Rg(mf)^T = Rg(mf)$

c. Hallar una base de $Nuf$

    Tenemos que resolver el sistema dado por $\left[mf | 0_{R^m}\right]$

## Ejercicio 3

Tenemos $f : R^3 \to R^3$ TL, $mf = \begin{bmatrix}
2 & 0 & 0 \\
3 & -1 & 1 \\
1 & 2 & 2
\end{bmatrix}$.
Calcular $DimImf$

$DimImf = Rg(mf)$

Luego podemos calcular la dimensión de la imagen, que nos permite ver si $f$
es **epimorfismo** Además como la dimensión del dominio y el codominio son
iguales, sabemos que $f$ es **isomorfismo**

