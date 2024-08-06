---
layout: post
title: Ajuste de Curvas por Método de Mínimos Cuadrados
author: Alan Yahir Juárez Rubio

categories:
  - matematicas
  - metodos-numericos
tags:
  - regla-falsa
  - falsa-posicion

date: 2023-10-29
last_updated: 2024-07-25 23:21

toc:
  beginning: true

pretty_table: true
---

La propiedad fundamental de este método es que la suma de los cuadrados de los
errores se hace tan pequeña como sea posible. Su popósito es encontrar la
ecuación que proporcionla la **desviación promedio** más cercana a cero. Para
que esto funcione se emplea la **técnica de máximos y mínimos**.

Para realizar el _ajuste polinomial_ se resuelve el siguiense sistema de
ecuaciones:

$$
\begin{matrix}
  \sum y    &=& a_0n         &+& a_1 \sum x       &+& a_2 \sum x^2     &+ \cdots +& a_n     \sum x^n \\
  \sum xy   &=& a_0 \sum x   &+& a_1 \sum x^2     &+& a_2 \sum x^3     &+ \cdots +& a_{n+1} \sum x^{n+1} \\
  \sum x^2y &=& a_0 \sum x^2 &+& a_1 \sum x^3     &+& a_2 \sum x^4     &+ \cdots +& a_{n+2} \sum x^{n+2} \\
  \vdots    &=& \vdots       & & \vdots           & & \vdots           &          & \vdots \\
  \sum x^ny &=& a_0 \sum x^n &+& a_1 \sum x^{n+1} &+& a_2 \sum x^{n+2} &+ \cdots +& a_{n+2} \sum x^{2n} \\
\end{matrix}
$$

## Ejemplo

Realice el ajuste lineal y cuadrático con los datos de la siguiente tabla

|   n   |  x  |  y  | x² | xy  | x²y | x³ | x⁴ |
| :---: | :-: | :-: | :-: | :-: | :--: | :-: | :-: |
|   1   | -3  | -27 |  9  | 81  | -243 | -27 | 81  |
|   2   | -2  | -16 |  4  | 32  | -64  | -8  | 16  |
|   3   | -1  | -9  |  1  |  9  |  -9  | -1  |  1  |
|   4   |  0  |  1  |  0  |  0  |  0   |  0  |  0  |
|   5   |  1  |  8  |  1  |  8  |  8   |  1  |  1  |
|   6   |  2  | 18  |  4  | 36  |  72  |  8  | 16  |
|   7   |  3  | 26  |  9  | 78  | 234  | 27  | 81  |
| Total |  0  |  1  | 28  | 244 |  -2  | -0  | 196 |

### Ajuste lineal

$$
\begin{cases}
  1   &=& 7a_0 &+& 0a_1 \\
  244 &=& 0a_0 &+& 28a_1
\end{cases} \tag{grado 1}
\Rightarrow
\begin{pmatrix}
  a_0 &=& \frac {3}{7}  &\approx& 0.14286 \\
  a_1 &=& \frac {61}{7} &\approx& 8.71429 \\
\end{pmatrix}
$$

$$y = 0.14268 + 8.71429x \tag{Ajuste lineal}$$

> ##### RESULTADO
>
> $$y(1.7) = 14.95715$$
{: .block-tip }

### Ajuste cuadrático

$$
\begin{cases}
  1   &=& 7a_0  &+& 0a_1  &+& 28a_2 \\
  244 &=& 0a_0  &+& 28a_1 &+& 0a_2 \\
  -2  &=& 28a_0 &+& 0a_1  &+& 196a_2
\end{cases} \tag{grado 3}
\Rightarrow
\begin{pmatrix}
  a_0 &=& \frac {3}{7}   &\approx& 0.14286 \\
  a_1 &=& \frac {61}{7}  &\approx& 8.71429 \\
  a_1 &=& -\frac {1}{14} &\approx& -0.07143
\end{pmatrix}
$$

$$y = 0.42857 + 8.71429x - 0.07143x^2 \tag{Ajuste cuadrático}$$

> ##### RESULTADO
>
> $$y(1.7) = 15.03643$$
{: .block-tip }
