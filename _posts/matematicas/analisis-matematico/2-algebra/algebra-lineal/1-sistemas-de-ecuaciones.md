---
title: Sistemas de Ecuaciones
author: Alan Yahir Juárez Rubio

aliases: Sistemas de ecuaciones lineales
tags: algebra, lineal, ecuaciones, sutitucion, igualacion, grafica, transformaciones elementales, sistema, ecuaciones, gauss

creation date: 22-04-2023
last modification date: 25-04-2023

type: Note
---

## Sistemas de ecuaciones

### Sistemas de ecuaciones 2x2

Un **sistema de ecuaciones** es aquel en el que hay _dos o más ecuaciones las cuales comparten entre sí los valores de las incógnitas_.

Un _sistema de ecuaciones lineales 2x2_ se representa de la siguiente manera:

$$
\begin{bmatrix}
ax & + &by & = &c\\
dx & + &ey & = &f
\end{bmatrix} =
\
\left[ \begin{array}{cc|c}
ax & by & c\\
dx & ey & f
\end{array} \right] =
\
\left[ \begin{array}{cc|c}
a & b & c\\
d & e & f
\end{array} \right] \tag{1}
$$

En la que la columna uno representa la primera incógnita ($x$), la columna dos la segunda incógnita ($y$) y la columna tres el resultado de cada fila, de cada ecuación.

#### Por sustitución

1. Se despeja una de las variables de alguna de las ecuaciones.
2. Se sustituye el valor de la variable encontrada en la otra ecuación y después despejarla.
3. Se sustituye el valor de la incógnita encontrada en cualquiera de las dos ecuaciones.
4. Se despeja para encontrar el valor de la incógnita faltante.
5. Comprobación.

#### Por igualación

1. Se despeja una variable de ambas ecuaciones.
2. Se iguala los valores de los despejes de dichas variables y se depeja la variable contraria.
3. Se sustituye la segunda variable en cualquiera de los despejes.
4. Se despeja la variable faltante para encontrar la solución
5. Comprobación.

#### Por gráfica

1. Se despeja de ambas ecuaciones la variable $y$.
2. Se tabulan ambos valores de $y$
   - Si es una _ecuación lineal_ basta con tabular solo 2 valores
3. Se agregan las coordenadas en el plano y se unen secuencialemente las de la ecuación 1 entre sí y las de la ecuación 2 entre sí.
   - Si es una _ecuación lineal_ se extiende la recta formada.
4. Analizar: las _intersecciones_ entre las _gráficas_ son las _soluciones del sistema_.

| Casos | Recta                   | Gráfica                                       | Cantidad de soluciones                                   |
| :---: | ----------------------- | --------------------------------------------- | -------------------------------------------------------- |
|   1   | Misma recta             | Misma gráfica                                 | Infintas soluciones                                      |
|   2   | Rectas paralelas        | Misma gráfica, pero con desplazamiento en $x$ | Sin soluciones                                           |
|   3   | Dos rectas no paralelas | -                                             | Única solución                                           |
|   4   | -                       | Dos gráficas distintas                        | Depende del número de intersecciones entre las gráficas. |

### Sistemas de ecuaciones lineales con más de dos variables

Un _sistema de ecuaciones_ se define de la siguiente manera

$$
A =\left[\begin{array}{cccc|cc}
\
a_{11}x_{1} & a_{12}x_{1} & \cdots & a_{1n}x_{1}  & k_1\\
a_{21}x_{2} & a_{22}x_{2} & \cdots & a_{2n}x_{2}  & k_2\\
\vdots      & \vdots      & \vdots & \ddots       & \vdots\\
a_{m1}x_{m} & a_{m2}x_{m} & \cdots & a_{mn}x_{n} & k_n\\
\end{array} \right] =
\
\left[\begin{array}{cccc|cc}
a_{11} & a_{12} & \cdots & a_{1n} & k_1\\
a_{21} & a_{22} & \cdots & a_{2n} & k_2\\
\vdots & \vdots & \vdots & \ddots & \vdots\\
a_{m1} & a_{m2} & \cdots & a_{mn} & k_n
\
\end{array} \right] \tag{2}
$$

en dónde $n$ representa la _cantidad de variables_ y $m$ la _cantidad de ecuaciones_.

#### Transformaciones elementales de una matriz

Dada una matriz de un sistema de ecuaciones lineales, una matriz de un sistema equivalente resulta si

1. Se intercambian dos renglones.
2. Se multiplica o divide un renglón por una constante diferente de cero.
3. Un múltiplo constante de un renglón se suma a otro renglón.

#### Gauss

El método de **Gauss** consiste en utilizar las **transformaciones elementales** para transformar un _sistema de ecuaciones lineales_ a su _forma escalonada_. Para después terminar de resolverla con cualquier otro método.

En el caso de _sistemas de ecuaciones lineales_ donde $m \geq n$

$$
A =
\left[\begin{array}{ccccc|c}
a_{11} & a_{12} & a_{12} & \cdots & a_{1n} & k_1\\
a_{21} & a_{22} & a_{23} & \cdots & a_{2n} & k_2\\
a_{31} & a_{32} & a_{33} & \cdots & a_{3n} & k_2\\
\vdots & \vdots & \vdots & \ddots & \vdots & \vdots\\
a_{m1} & a_{m2} & a_{m3} & \cdots & a_{mn} & k_m\\
\end{array} \right] =
\
\left[\begin{array}{ccccc|c}
1      & P(a_{12})   & P(a_{13}) &  \cdots & P(a_{1n}) & P(k_1) \\
0      & 1           & P(a_{23}) & \cdots & P(a_{2n}) & P(k_2)\\
0      & 0           & 1         & \cdots & P(a_{3n}) & P(k_3)\\
\vdots & \vdots      & \vdots    & \ddots & \vdots    & \vdots\\
0      & 0           & 0         & \cdots & Q         & P(k_{m})
\end{array} \right] \tag{3}
$$

- Si $n = m \to Q = 1$
- Si $n < m \to Q = 0$

En el caso de _sistemas de ecuaciones lineales_ donde $m < n$

$$
A=
\left[\begin{array}{ccccc|c}
a_{11} & a_{12} & a_{13} &  \cdots & a_{1n} & k_1\\
a_{21} & a_{22} & a_{23} & \cdots & a_{2n} & k_2\\
a_{31} & a_{32} & a_{33} & \cdots & a_{3n} & k_2\\
\vdots & \vdots & \vdots & \ddots & \vdots & \vdots\\
a_{m1} & a_{m2} & a_{m3} & \cdots & a_{mn} & k_m\\
\end{array} \right] =
\
\left[\begin{array}{cccccc|c}
1      & P(a_{12})   & P(a_{13}) & P(a_{14}) & \cdots & P(a_{1n}) & P(k_1) \\
0      & 1           & P(a_{23}) & P(a_{24}) & \cdots & P(a_{2n}) & P(k_2)\\
0      & 0           & 0         & 1         & \cdots & P(a_{3n}) & P(k_3)\\
\vdots & \vdots      & \vdots    & \vdots    & \ddots & \vdots    & \vdots\\
0      & 0           & 0         & 0         & \cdots & P(a_{mn})         & P(k_{m})
\end{array} \right] \tag{4}
$$

> [!NOTE]
>
> - Sea $i$ una determinada fila y $j$ una determinada columna, entonces $P(a_{ij}) = (ba+ c)_{ij}$
> - En $(3)$ la _diagonal principal_ está conformada de unos y debajo de estos unos hay puros ceros
> - En $(4)$ la _cantidad de ceros_ antes del $1$ de cada fila, depende del _número de la fila $n$_. Se puede representar como: $2^{n-1}$

#### Gauss Jordan

El método de **Gauss Jordan** consiste en utilizar las **transformaciones elementales** para transformar un _sistema de ecuaciones lineales_ de manera que su _diagonal principal_ esté conformado de unos y el resto de la _matriz de coeficientes_ sean ceros. Este método no aplica para matrices con tamaño $m < n$

$$
A =
\left[\begin{array}{ccccc|c}
a_{11} & a_{12} & a_{12} & \cdots & a_{1n} & k_1\\
a_{21} & a_{22} & a_{23} & \cdots & a_{2n} & k_2\\
a_{31} & a_{32} & a_{33} & \cdots & a_{3n} & k_2\\
\vdots & \vdots & \vdots & \ddots & \vdots & \vdots\\
a_{m1} & a_{m2} & a_{m3} & \cdots & a_{mn} & k_m\\
\end{array} \right] =
\
\left[\begin{array}{ccccc|c}
1      & 0   & 0 &  \cdots & 0 & P(k_1) \\
0      & 1           & 0 & \cdots & 0 & P(k_2)\\
0      & 0           & 1         & \cdots & 0 & P(k_3)\\
\vdots & \vdots      & \vdots    & \ddots & \vdots    & \vdots\\
0      & 0           & 0         & \cdots & Q         & P(k_{m})
\end{array} \right] \tag{5}
$$

- Si $n = m \to Q = 1$
- Si $n < m \to Q = 0$
