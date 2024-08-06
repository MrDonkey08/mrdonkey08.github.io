---
layout: post
title: Conjunto Fundamental de Soluciones
author: Alan Yahir Juárez Rubio

categories:
  - matematicas
  - ecuaciones-diferenciales
tags:
  - ecuacion-diferencial-lineal
  - principio-de-superposicion

date: 11-04-2023
last_updated: 11-04-2023

toc:
  sidebar: right
---

Consideremos **una ecuación diferencial lineal homogénea de coeficientes
constantes**, es decir, una ecuación de la forma:

$$
  a_ny^{(n)} + a_{n-1}y^{(n-1)} + \cdots + a_{2}y\: '' + a_{1}y\: ' + a_0y = 0
  \tag{1}
$$

donde $$ a_n,\dots, a_0 $$ son números constantes.

## Teorema

La ecuación $$ (1) $$ tiene exactamente $$ n $$ soluciones $$ f*1,\dots,f_n $$
que son \_linealmente independientes entre sí*. En este caso, la solución
general de $$ (1) $$ es de la forma:

$$y = C_1f_1 + C_2f_2 +\cdots + C_nf_n \tag{2}$$

donde $$ C_1, \dots, C_n $$ son parámetros constantes.

Llamaremos al conjunto de funciones $$ \{f_1,\dots, f_n \} $$ el **conjunto
fundamental de soluciones** de $$ (1) $$.

## Teorema (Principio de superposición)

1. Si $$ f_1, f_2,\dots, f_k $$ son soluciones de $$ (1) $$ y
   $$ C_1,\dots, C_k $$ son constantes, entonces la función
   $$ C_1f_1 + C_2f_2 + \cdots + C_kf_k $$ también es una solución de
   $$ (1) $$.

2. Si $$ f_1, f_2,\dots, f_k $$ son $$ n $$ soluciones y son linealmente
   independiendes, entonces la solución general de $$ (1) $$ es:

$$y = C_1f_1 + C_2f_2 +\cdots + C_nf_n$$

donde $$ C_1, \dots, C_n $$ son parámetros constantes.

---

Consideremos una **ecuación diferencial lineal homogénea de coeficientes
constantes de orden $$ n $$**, es decir, una ecuación de la forma:

$$
  a_ny^{(n)} + a_{n-1}y^{(n-1)} + \cdots+ a_{2}y\: '' + a_{1}y\: ' + a_0y = 0
  \tag{1}
$$

donde $$ a_n,\dots, a_0 $$ son números constantes. Asociada a esta ecuación
diferencial tenemos la **ecuación algebraíca**:

$$
a_nt^{(n)} + a_{n-1}t^{(n-1)} +\cdots+ a_{2}t^2 + a_{1}t + a_0 = 0
\tag{2}
$$

Asumamos que hemos resuelto la ecuación $$ (2) $$. Entonces por cada solución
de $$ (2) $$ añadiremos una o varias funciones al conjunto fundamental de
soluciones de la siguiente manera:

- Por cada **solución real $$ t=a $$** de **multiplicidad $$ k $$**,
  añadiremos al c.f.s. Las funciones:

  $$e^{ax}, xe^{ax}, \dots, x^{k-1}e^{ax}$$

- Por cada **par de soluciones complejas** de la forma $$ t = a \pm bi $$,
  ambas

soluciones $$ k $$, añadiremos al c.f.s. las funciones

$$e^{ax}\cos(bx), xe^{ax}\cos(bx), \dots, x^{k-1}e^{ax}\cos(bx)$$

$$e^{ax}\sin(bx), xe^{ax}\sin(bx), \dots, x^{k-1}e^{ax}\sin(bx)$$
