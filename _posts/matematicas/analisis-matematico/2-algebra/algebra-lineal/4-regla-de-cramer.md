---
title: Regla de cramer
author: Alan Yahir Juárez Rubio

tags: algebra, lineal, cramer, determinantes, sistema, ecuaciones, matriz

creation date: 22-04-2023
last modification date: 01-10-2023

type: Note
---

## Regla de Cramer

La **regla de cramer** se utiliza para conseguir la solución de un _sistemas de ecuaciones lineales de tamaño $n\times n$_ mediante el cálculo de **determinantes**.

$$
D =\left[\begin{array}{cccc|cc}
\
a_{11}x_{1} & a_{12}x_{1} & \cdots & a_{1n}x_{1}  & k_1\\
a_{21}x_{2} & a_{22}x_{2} & \cdots & a_{2n}x_{2}  & k_2\\
\vdots      & \vdots      & \vdots & \ddots       & \vdots\\
a_{n1}x_{n} & a_{n2}x_{n} & \cdots & a_{nn}x_{n} & k_n\\
\end{array} \right] \tag{1} =
\
\left[\begin{array}{cccc|cc}
a_{11} & a_{12} & \cdots & a_{1n} & k_1\\
a_{21} & a_{22} & \cdots & a_{2n} & k_2\\
\vdots & \vdots & \vdots & \ddots & \vdots\\
a_{n1} & a_{n2} & \cdots & a_{nn} & k_n
\
\end{array} \right]
$$

1. Se calcula el _**determinante** de la matriz original_ ($|D|$), es decir

$$
|D| = \begin{vmatrix}
a_{11} & a_{12} & \cdots & a_{1n}\\
a_{21} & a_{22} & \cdots & a_{2n}\\
\vdots & \vdots & \ddots & \vdots\\
a_{n1} & a_{n2} & \cdots & a_{nn}\\
\end{vmatrix} \tag{2}
$$

> [!IMPORTANT] Importante
>
> - Si $|D| = 0$, no se puede aplicar la **regla de cramer**. Provoca _indeterminación _$\frac{a}{0}$
> - Si $|D| \neq 0$, se puede aplicar la **regla de cramer**.

2. Después se calcula los _determinantes con respecto a las variables_ ($x_{1}, x_{2},\dots x_{n}$)

$$
\begin{array}{cc}
\
|D_{x_{1}}| = \begin{vmatrix}
k_{1}  & a_{12} & a_{13} & \cdots & a_{1n}\\
k_{2}  & a_{22} & a_{23} & \cdots & a_{2n}\\
\vdots & \vdots & \vdots & \ddots & \vdots\\
k_{n}  & a_{n1} & a_{n2} & \cdots & a_{nn}\\
\end{vmatrix},\;
\
|D_{x_{2}}| = \begin{vmatrix}
a_{11} & k_{1}  &   a_{13} & \cdots & a_{1n}\\
a_{21} & k_{2}  &   a_{23} & \cdots & a_{2n}\\
\vdots & \vdots & \vdots   & \ddots & \vdots\\
a_{n1} & k_{n}  &   a_{n3} & \cdots & a_{nn}\\
\end{vmatrix},\;\\\\
\
|D_{x_{3}} |= \begin{vmatrix}
a_{11} & a_{12} & k_{1}  & a_{14} & \cdots & a_{1n}\\
a_{21} & a_{22} & k_{2}  & a_{24} & \cdots & a_{2n}\\
\vdots & \vdots & \vdots & \vdots & \ddots & \vdots\\
a_{n1} & a_{n2} & k_{n}  & a_{n4} & \cdots & a_{nn}\\
\end{vmatrix},\; \cdots\;
\
|D_{x_{n}}| = \begin{vmatrix}
a_{11} & a_{12} & \cdots & a_{1n-1} & k_{1}\\
a_{21} & a_{22} & \cdots & a_{2n-1} & k_{2}\\
\vdots & \vdots & \vdots & \ddots   & \vdots\\
a_{n1} & a_{n2} & \cdots & a_{nn-1} & k_{n}\\
\end{vmatrix} \tag{3}
\
\end{array}
$$

> [!ABSTRACT] Observación
>
> Como se puede apreciar en $(3)$, para un _determinante con respecto a $x_{c}$ variable\_ (donde $c$ es la columna a la que pertenece en a $(1)$), se reemplaza la columna ($c$) por la columna de las soluciones ($k$) y el resto se mantiene igual que en $(1)$.

3. Utilizar la siguiente _fórmula_ para conseguir la _solución del sistema de ecuaciones_

$$x_{1}=\frac{|D_{x_{1}}|}{|D|},\; x_{2}=\frac{|D_{x_{2}}|}{|D|},\; \cdots\; x_{n}=\frac{|D_{x_{n}}|}{|D|}, \text{ donde |D|} \neq 0 \tag{4}$$

<!---
<div style="page-break-after: always;"></div>

---
## Referencias

- W., E. y A., J. (2009). Encontrar el determinante de una matriz (12<sup>a</sup> ed.). En S. R. Cervantes (Ed.), _Álgebra y trigonometría con geometría análitica_ (pp. 715-717). Editorial CENGAGE Learning.

--->
