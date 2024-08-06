---
layout: post
title: Variación de Parámetros
author: Alan Yahir Juárez Rubio

categories:
  - matematicas
  - ecuaciones-diferenciales
tags:
  - ed-lineal-no-homogenea

date: 11-04-2023
last_updated: 11-04-2023

toc:
  sidebar: right
---

Consideremos una **ecuación diferencial lineal no-homogénea** de la forma:

$$
a_ny^{(n)} + a_{n-1}y^{(n-1)} +\cdots+ a_{2}y\: '' + a_{1}y\: ' + a_0y = f(x)
\tag{1}
$$

donde $$ a_n,\dots, a_0 $$ son números constantes. Asociada a esta ecuación
diferencial tenemos la **ecuación algebraíca**:

$$
a_ny^{(n)} + a_{n-1}y^{(n-1)} + \cdots + a_{2}y\:'' + a_{1}y\:' + a_0y = 0
\tag{2}
$$

Entonces la solución general de $$ (1) $$ es de la forma:

$$y = y_h + y_p$$

donde $$ y_h $$ es la solución de $$ (2) $$, llamada la **solución auxiliar**
y $$ y_p $$ es una solución de $$ (1) $$, que llamamos **solución particular**.

Para determinar la **solución particular**, existen diferentes métodos, el que
veremos a continuación se llama **variación de parámetros**.

Sabemos que la **solución auxiliar** es de la forma:

$$y_h = C_1f_1 + C_2f_2 + \dots + C_nf_n$$

donde $$ C_1, \dots, C_n $$ son parámetros constantes y
$$ \{f_1, \dots, f_n\} $$ es el conjunto fundamental de soluciones para la
**ecuación homogénea** $$ (2) $$. Entonces la **solución particular** es de la
forma:

$$y_p = u_1f_1 + u_2f_2 + \dots + u_nf_n$$

donde ahora $$ u_1, \dots u_n $$ son funciones, y estas se obtienen al resolver
un sistema de ecuaciones.

Si la ecuación es de orden 2, entonces obtenemos $$ u_1 $$ y $$ u_2 $$
resolviendo el sistema:

$$
\begin{array}{c}
  u_1\:'f_1    & + & u_2\:'f_2    & = & 0 \\
  u_1\:'f_1\:' & + & u_2\:'f_2\:' & = & g(x)
\end{array}
$$

Si la ecuación es de orden 3, obtenemos $$ u_1 $$, $$ u_2 $$ y $$ u_3 $$
resolviendo el sistema:

$$
\begin{array}{c}
  u_1\:'f_1     & + & u_2\:'f_2     & = & 0 \\
  u_1\:'f_1\:'  & + & u_2\:'f_2\:'  & = & 0 \\
  u_1\:'f_1\:'' & + & u_2\:'f_2\:'' & = & g(x)
\end{array}
$$

El sistema es análogo para ecuaciones de grado superior:

Notemos que al resolver el sistema se obtiene las derivadas de $$ u_1, \dots,
u_n $$, por lo que posteriormente se debe intregrar.
