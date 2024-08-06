---
layout: post
title: Determinantes
author: Alan Yahir Juárez Rubio

categories:
  - matematicas
  - algebra-lineal
tags:
  - determinantes
  - gauss
  - sarrus
  - laplace
  - inversa
  - menor
  - cofactor
  - adjunta
  - triangular

date: 2023-04-22 15:22
last_updated: 2024-04-25

toc:
  beginning: true
---

El **determinate** es una función que se le aplica solamente a _matrices
cuadradas_ y puede ser expresado como:

$$det(A), |A| \tag{1}$$

y sustituyendo cada corchete de la matriz por una línea

> ##### IMPORTANTE
>
> En un sistema homogéneo
>
> - Si $$ |D| = 0 \to D $$ es **linealmente dependiente**, es decir, tiene _0 o
>   infinitas soluciones_.
> - Si $$ |D| \neq 0 \to D $$ es **linealmente independiente**, es decir, tiene
>   _solución única_.
{: .block-important }

## Menores y Cofactores

$$
\begin{array}{ccccc}
  \text{Matriz} & \text{Menor} &\text{Cofactor o Adjunto}
  \\
  \begin{bmatrix} \cancel{a_{11}} & \cancel{a_{12}} & \cancel{a_{13}} & \cancel{\cdots} & \cancel {a_{1n}} \\
    \cancel{a_{21}}               & a_{22}          & a_{23}          & \cdots & a_{2n} \\
    \cancel{a_{31}}               & a_{32}          & a_{33}          & \cdots & a_{3n} \\
    \cancel{\vdots}               & \vdots          & \vdots          & \ddots & \vdots \\
    \cancel{a_{m1}}               & a_{m2}          & a_{m3}          & \cdots & a_{mn} \\
  \end{bmatrix}
  \ & M_{11} =
  \begin{vmatrix}
    a_{22} & a_{23} & \cdots & a_{2n} \\
    a_{32} & a_{33} & \cdots & a_{3n} \\
    \vdots & \vdots & \ddots & \vdots \\
    a_{m2} & a_{m3} & \cdots & a_{mn} \\
  \end{vmatrix}
  \
  & A_{11} = (-1)^{1+1}M_{11}
  \
\end{array} \tag{2}
$$

Sea $$ i $$ la fila y $$ j $$ la columna a la que pertenece un elemento,
la _**menor** de un elemento_ es el **determinante** que se obtiene al eliminar
la fila y columna de la matriz original al que pertenece dicho elemento. Por
otra parte, el _**cofactor** de un elemento_ es el resultado de elevar $$ -1 $$
a la ( $$ i + j $$ ).

Otra manera de determinar el signo dado de por $$ (-1)^{i+j} $$ es considerar el
siguiente tablero de signos.

$$
\begin{bmatrix}
  +      & -      & +      & -      & \cdots \\
  -      & +      & -      & +      & \cdots \\
  +      & -      & +      & -      & \cdots \\
  -      & +      & -      & +      & \cdots \\
  \vdots & \vdots & \vdots & \vdots
\end{bmatrix} \tag{3}
$$

## Determinantes

### Regla de Laplace

La siguiente fórmula sirve para calcular **determinates** de _matrices
cuadradas de cualquier orden_, pero se suele utilizar para las de orden 4 en
adelante. Para las de orden 2 y 3 existen fórmulas más simples que derivan de
esta, tal como la **regla de sarrus**.

$$|A| = a_{11}A_{11} + a_{12}A_{12} + \cdots + a_{1n}A_{1n} \tag{4}$$

o expresado en términos de **cofactores**:

$$|A| = a_{11}M_{11} - a_{12}M_{12} + \cdots + a_{1n}(-1)^{1+n}M_{1n} \tag{5}$$

**Determinantes de matrices 2x2**: La mutlplicación de la diagonal principal
menos la multiplicación de la diagonal secundaria:

$$
|A| =
\begin{vmatrix}
  a_{11} && a_{12} \\
  \\
  a_{21} && a_{22} \\
\end{vmatrix}\Rightarrow
\
\begin{bmatrix}
  a_{11} && a_{12} \\
    &\color{red}{\searrow}\hspace{-10pt}\color{blue}{\nearrow} \\
  a_{21} && a_{22}
\end{bmatrix} = \color{red}{a_{11}a_{12}} \color{gray}{-}
\color{blue}{a_{21}a_{22}}
$$

### Regla de Sarrus

La **regla de sarrus** solo se utiliza para calcular **determinantes de
matrices 3x3**. Consiste en extender la matriz hacia la derecha con las
primeras dos filas y sumar la multiplicación de la diagonal principal de cada
$$ a*1j $$ y a eso restarle la suma de los productos de las diagonaleIs
secundarias de cada $$ a*{3j} $$ .

$$
|A| =\begin{vmatrix}
  a_{11} && a_{12} && a_{13} \\
  \\
  a_{21} && a_{22} && a_{23} \\
  \\
  a_{31} && a_{32} && a_{33} \\
\end{vmatrix}\Rightarrow
\
\left[\begin{array}{cccccc|ccc}
  a_{11} && a_{12} && a_{13} && a_{11} && a_{12}
  \\
  &\color{red}{\searrow}\hspace{-10pt}
    && \color{red}{\searrow}\hspace{-10pt}\color{blue}{\nearrow}
    && \color{red}{\searrow}\hspace{-10pt}\color{blue}{\nearrow}
    && \color{blue}{\nearrow}
  \\
  a_{21} && a_{22} && a_{23} && a_{21} && a_{22}
  \\
  &\color{blue}{\nearrow}
    && \color{red}{\searrow}\hspace{-10pt}\color{blue}{\nearrow}
    && \color{red}{\searrow}\hspace{-10pt}\color{blue}{\nearrow}
    && \color{red}{\searrow} \\
  \
  a_{31} && a_{32} && a_{33} && a_{31} && a_{32}
\end{array}\right] \tag{6}
$$

$$
|A| =
  {\color{gray} (
    {\color{red}{a_{11}a_{22}a_{33}}}
      +
    {\color{red}{a_{12}a_{23}a_{31}}}
      +
    {\color{red}{a_{13}a_{21}a_{32}}}
  ) - (
    {\color{blue}{a_{31}a_{22}a_{13}}}
      +
    {\color{blue}{a_{32}a_{23}a_{11}}}
      +
    {\color{blue}{a_{33}a_{21}a_{12}}}
  )}
\tag{7}
$$

<!-- 123, 231, 312 -->

### Método de Eliminación de Gauss

El **método de operaciones elementales** consiste en tranformar una _matriz
cuadrada_ determinada en una **matriz triangular de ceros**

El **determinante** de una **matriz triangular de ceros** es igual al producto
de los elementos de la **diagonal principal**. Esto debido a que, al efectuar
la **regla de Laplace** $$ (3) $$ , el único producto que no se hace 0 es el de
la **diagonal principal**.

$$
\begin{array}{ccc}
  \text{Matriz} && \text{Matriz triangular superior}
  \\
  \begin{vmatrix}
    a_{11} & a_{12} & \cdots & a_{1n} \\
    a_{21} & a_{22} & \cdots & a_{2n} \\
    \vdots & \vdots & \ddots & \vdots \\
    a_{n1} & a_{n2} & \cdots & a_{mn}
    \\
  \end{vmatrix}
  \ & = &
  \begin{vmatrix}
    P(a_{11}) & P(a_{12}) & \cdots & P(a_{1n}) \\
    0         & P(a_{22}) & \cdots & P(a_{2n}) \\
    \vdots    & \vdots    & \ddots & \vdots \\
    0         & 0         & 0      & P(a_{nn})
  \end{vmatrix}\tag{8}
  \\ \\
  & = &
    P(a_{11}) \cdot P(a_{22}) \cdot {\dots} \cdot P(a_{nn})
\end{array}
$$
