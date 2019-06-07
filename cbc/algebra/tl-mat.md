# Def TL
dada $f : V \to W$, con $V, W$ espacios vectoriales, $f$ es **transformación
lineal** si y sólo si:

* $f(a+b) = fa + fb \quad \forall a,b \in V$
* $f(\lambda b) = \lambda (fb) \quad \forall a \in V, \lambda \in R$

## Prop

Si $M \in R^{m\times n}$, luego $f : R^n \to R^m, fv = Mv$ es una *TL*

### Demo

* $f(a + b) = M(a+b) = Ma + Mb = fa + fb$
* $f(\lambda a) = M(\lambda a) = \lambda (Ma) = \lambda (fa)$

# Def Matriz de una TL de Rn a Rm

Si $f : R^n \to R^m$ *TL*

Se define $mf = \left[fE_1|fE_2|\dots |fE_m\right] \in R^{m \times n}$,
donde $E$ es la base canónica de $R^n$

## Prop

Se cumple que aplicar $f$ es lo mismo que multiplicar por $M$, es decir
$fv = (mf)v \quad \forall v \in V$

### Demo

Notemos que anda para la base canónica, y como producto por matriz es una
*TL* ya está

## Prop

Si $f : R^n \to R^m$ *TL*, luego $Dim \; Imf = Rg \; mf$

### Demo

Notemos que $Im \; f$ es el generado por $\langle fE_i \rangle$, con $E$
alguna base, en particular la canónica. Pero $fE_i$ son las columnas de
$mf$, entonces para sacar una base de $Im \; f$ triangulamos y sacamos el
$Rg$ de $(mf)^T$, pero el $Rg$ de una matriz no cambia al transponer

## Prop

Si $f : R^n \to R^m$ *TL*, luego $Dim \; Nu f = n - Rg \; mf$

## Prop

$f : R^n \to R^n$ *TL* es *isomorfismo* si y solo si $mf$ es invertible

# Def matriz de una TL

Sea $B = \{v_1, v_2, \dots, v_n\}$ una base de $V$

Sea $B' = \{w_1, w_2, \dots, w_m\}$ una base de $W$

Si $f : V \to W$, **defino**

$M_{BB'}f = \left[(fv_1)_{B^'} \; |\; (fv_2)_{B^'} \; |\; \dots \;|\; (fv_n)_{B^'}\right] \in R^{m \times n}$

## Prop

$(M_{BB^'}f)(v_B) = (fv)_{B^'}$

## Prop

Cuando $f : R^n \to R^m$ *TL*, entonces
$M_{EE^'}f = mf$

## Prop

$f : V \to W$ es *iso* si y sólo si $M_{BB^'}f$ es inversible para algunas
bases $B$ y $B'$

## Prop

El rango de $M_{BB^'}f$ no depende de la elección de bases $B$, $B'$

## Prop

Podemos hacer esto para las matrices de $R^{m \times n}$ tomándonos su base
canónica

## Notación

Cuando $f : V \to V$, y $B$ base de $V$ podemos escribir

$M_Bf = M_{BB}f$

