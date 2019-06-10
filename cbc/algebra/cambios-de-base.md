# Hacer que la Matriz de la tranf. sea I

Si tenemos $f : V \to W$ *TL iso* y alguna base $B = \{v_1, \dots, v_n\}$,
entonces tomémonos $B^' = \{fv_i\}$, luego la matriz queda:

$M_{BB^'}f = I$, ya que $B^'$ es base

# Def TL Nula

Si tenemos $N : V \to W$, $Nv = \bar 0 \quad \forall v$, $N$ se llama la
*TL* nula

Tenemos $M_{BB^'}f = 0_{m \times n}$

# Def TL Identidad
Si tenemos $id : V \to V$, $id \; v = v \quad \forall v$, entonces $id$ es
la *TL* identidad.

Se cumple $M_B \; id = I_{n \times n} \quad \forall B$ base de $V$

## Prop

$M_{BE} \; id = [B_1 \mid B_2 \mid \dots \mid B_n]$, que cumple
$M_{BE} \cdot (v_B) = v$

$M_{EB} \; id = [B_1 \mid B_2 \mid \dots \mid B_n]^{-1}$, que cumple
$M_{BE} \cdot (v) = v_B$

# Matriz de la composición

Sea $f : R^n \to R^m$ *TL* y $\; g : R^m \to R^k$ *TL*

Tenemos $g \circ f : R^n \to R^k$, y se cumple:

$m\; (g \circ f) = mg \cdot mf$. Demo trivial

## En gral

Sea $f : V \to W$ *TL*, y $g : W \to U$ TL.
Y sean $B$, $B^'$ y $B^{''}$ bases de $V$, $W$, $U$

Entonces $M_{BB^{''}}(g \circ f) = (M_{B^'B^{''}}\;g) \cdot (M_{BB^'}\;f)$

### Corolario

$g \circ f$ *iso* $\iff$ $f$ *iso* y $g$ *iso*

# Matriz de la inversa

$M_{B^'B} \;\left(f^{-1}\right) = \left(M_{BB^'}\;f\right)^{-1}$

## Demo

Notemos que $f \circ f^{-1} = id$, luego

$M_{B'}\;(f \circ f) = I$, entonces
$M_{BB^'} \;f \cdot B_{B^'B}\;f^{-1} = I$, y ya está

# Cambio de base

Sean $B$, $B'$ bases de $V$, luego se **define**:

$C_{BB'} = M_{BB^'}\;id  \;\in R^{n \times n}$, es decir

$C_{BB^'} = \left[(B_i)_{B^'}\mid \dots\right]$

## Componer con cambios de base

Si se tiene $g : V \to U$ y $f : U \to W$, luego, para cualquiera
$A$ base de $V$, bases $B$, $D$ de $U$, y base $F$ de $W$, luego:

$M_{AF}\;(f \circ g) = M_{DF} \;f \cdot C_{BD} \cdot M_{AB} \; g$
