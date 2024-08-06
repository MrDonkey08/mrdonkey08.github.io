---
layout: post
title: Regla de Cramer
author: Alan Yahir Juárez Rubio

categories:
  - matematicas
  - algebra-lineal
tags:
  - algebra
  - lineal
  - cramer
  - determinantes
  - sistema
  - ecuaciones
  - matriz

date: 2023-04-22 19:52
last_updated: 2024-04-25
---

La **regla de cramer** se utiliza para conseguir la solución de un _sistemas de
ecuaciones lineales de tamaño $$ n\times n $$_ mediante el cálculo de
**determinantes**.

$$
D =
\left[\begin{array}{cccc|cc}
  a_{11}x_{1} & a_{12}x_{1} & \cdots & a_{1n}x_{1} & k_1\\
  a_{21}x_{2} & a_{22}x_{2} & \cdots & a_{2n}x_{2} & k_2\\
  \vdots      & \vdots      & \vdots & \ddots      & \vdots\\
  a_{n1}x_{n} & a_{n2}x_{n} & \cdots & a_{nn}x_{n} & k_n\\
\end{array} \right] \tag{1} =
\
\left[\begin{array}{cccc|cc}
  a_{11} & a_{12} & \cdots & a_{1n} & k_1\\
  a_{21} & a_{22} & \cdots & a_{2n} & k_2\\
  \vdots & \vdots & \vdots & \ddots & \vdots\\
  a_{n1} & a_{n2} & \cdots & a_{nn} & k_n
\end{array} \right]
$$

- Se calcula el _**determinante** de la matriz original_ ($$ \mid D \mid $$),
  es decir:

$$
\mid D \mid =
\begin{vmatrix}
  a_{11} & a_{12} & \cdots & a_{1n}\\
  a_{21} & a_{22} & \cdots & a_{2n}\\
  \vdots & \vdots & \ddots & \vdots\\
  a_{n1} & a_{n2} & \cdots & a_{nn}\\
\end{vmatrix} \tag{2}
$$

> #### IMPORTANTE
>
> - Si $$ \mid D \mid = 0 $$, no se puede aplicar la **regla de cramer**. Provoca
_indeterminación_ $$ \frac{a}{0} $$
> - Si $$ \mid D \mid \neq 0 $$, se puede aplicar la **regla de cramer**.
{: .block-important }

- Después se calcula los _determinantes con respecto a las variables_
  ($$ x*{1}, x*{2},\dots x\_{n} $$)

$$
\begin{array}{cc}
\
 \mid D_{x_{1}} \mid =
\begin{vmatrix}
  k_{1}  & a_{12} & a_{13} & \cdots & a_{1n}\\
  k_{2}  & a_{22} & a_{23} & \cdots & a_{2n}\\
  \vdots & \vdots & \vdots & \ddots & \vdots\\
  k_{n}  & a_{n1} & a_{n2} & \cdots & a_{nn}\\
\end{vmatrix},\;
\
 \mid D_{x_{2}} \mid =
\begin{vmatrix}
  a_{11} & k_{1}  & a_{13} & \cdots & a_{1n}\\
  a_{21} & k_{2}  & a_{23} & \cdots & a_{2n}\\
  \vdots & \vdots & \vdots & \ddots & \vdots\\
  a_{n1} & k_{n}  & a_{n3} & \cdots & a_{nn}\\
\end{vmatrix},\;\\\\
\
 \mid D_{x_{3}} \mid =
  \begin{vmatrix}
  a_{11} & a_{12} & k_{1}  & a_{14} & \cdots & a_{1n}\\
  a_{21} & a_{22} & k_{2}  & a_{24} & \cdots & a_{2n}\\
  \vdots & \vdots & \vdots & \vdots & \ddots & \vdots\\
  a_{n1} & a_{n2} & k_{n}  & a_{n4} & \cdots & a_{nn}\\
\end{vmatrix},\; \cdots\;
\
 \mid D_{x_{n}} \mid =
\begin{vmatrix}
  a_{11} & a_{12} & \cdots & a_{1n-1} & k_{1}\\
  a_{21} & a_{22} & \cdots & a_{2n-1} & k_{2}\\
  \vdots & \vdots & \vdots & \ddots & \vdots\\
  a_{n1} & a_{n2} & \cdots & a_{nn-1} & k_{n}\\
\end{vmatrix} \tag{3}
\
\end{array}
$$

> ##### Observación
>
> Como se puede apreciar en $$ (3) $$, para un *determinante con respecto a
> $$ x\_{c} $$ variable\* (donde $$ c $$ es la columna a la que pertenece en
> $$ (1) $$), se reemplaza la columna ($$ c $$) por la columna de las
> soluciones ($$ k $$) y el resto se mantiene igual que en $$ (1) $$.
{: .block-abstract }

- Utilizar la siguiente _fórmula_ para conseguir la _solución del sistema de
  ecuaciones_

$$
x_{1} = \frac{ \mid D_{x_{1}} \mid }{ \mid D \mid },
x_{2} = \frac{ \mid D_{x_{2}} \mid }{ \mid D \mid }, \cdots
x_{n} = \frac{ \mid D_{x_{n}} \mid }{ \mid D \mid },
\text{ donde } \mid D \mid \neq 0
\tag{4}
$$

<div style="page-break-after: always;"></div>

---

## Referencias

- W., E. y A., J. (2009).
  Encontrar el determinante de una matriz
  (12<sup>a</sup> ed.).
  En S. R. Cervantes (Ed.),
  _Álgebra y trigonometría con geometría análitica_
  (pp. 715-717).
  Editorial CENGAGE Learning.
