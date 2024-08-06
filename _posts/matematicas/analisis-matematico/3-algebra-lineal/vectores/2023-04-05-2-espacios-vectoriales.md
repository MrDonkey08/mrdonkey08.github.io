---
layout: post
author: Alan Yahir Juárez Rubio
title: Guía de Estudio sobre Espacios Vectoriales

categories:
  - matematicas
  - algebra-lineal
tags:
  - vector
  - operaciones-basicas
  - multiplo-escalar

date: 2023-04-05

toc:
  sidebar: right
---

## Combinaciones lineales

$$x = c_1v_1 + c_2v_2 + \cdots + c_nv_n$$

## Espacio vectorial

### En ℝⁿ

Para determinar si una **combinación lineal** pertenece a **ℝⁿ**, nos
aseguramos que los vectores sean de dimensión $$ n $$

### Subespacio generador o conjunto generador

Sea $$ V $$ un **vector** y $$ S $$ un **espacio vectorial**, se dice que
$$ S $$ es un **subespacio generador** de $$ V $$ si existe una **combinación
lineal** que dé como resultado el vector $$ V $$

### Base

Sea $$ U $$ un **espacio vectorial** y $$ S $$ un **espacio vectorial**, se
dice que $$ S $$ es **base** de $$ U $$ si existe una **combinación lineal**
qué pueda dar como resultado cualquier **vector** de $$ U $$

<!-- Para determinar que $$ S $$ es **base** de $$ U $$ **combinación
lineal** y después sacar el **determinante** de la **combinación lineal**; si
este es diferente de cero, entonces $$ S $$ es **base** de $$ U $$, en caso
contrario, no lo es. -->

## Proyección de un ortogonal

### Producto Interno

Para espacios vectoriales

$$〈u, v〉 = u \cdot v$$

<!-- Espacios vectoriales, con funciones, matrices, reales, ecuaciones -->

**Ortogonal**: Cuando el ángulo es de 90°

### Proyección de un ortogonal

Sean $$ u $$ y $$ v $$ en un espacio $$ V $$ con producto interno, tal que
$$ V \neq \theta $$. La **proyección** de un **ortogonal** de $$ u $$ sobre
$$ v $$ está dada por:

$$\text{proy}_v = \frac{〈u, v〉}{〈v, v〉} v$$

**Ortogonal**: Producto punto tiene que dar 0.

## Bases Ortogonales y Ortonormales

Sea $$ S $$ un **conjunto** en un **espacio vectorial** $$ V $$ con **producto
interno**, se llama **ortogonal**, si todo par de vectores en $$ S $$ es
**ortogonal**. Si además, cada vector en $$ S $$ es unitario, se denomina
**ortonormal**

**Ortogonal:**

$$〈v_i, v_j〉 = 0, i \pm j$$

**Ortonormal:** **Ortogonal** y

$$
\displaylines{
  \| v_i \| = 1, &
  i = 1, 2, 3, \dots n
}
$$

### Proceso de Ortonormalización de Gram - Schmidt

Sea $$ B $$ una **base** del espacio $$ V $$ con **producto interno**

Sea $$ B\:' $$ una **base ortogonal** en $$ V $$ dado por:

$$
\begin{array}{ll}
  w_1 = v_1 \\
  w_2 = v_2 - \cfrac{〈v_2, w_1〉}{〈w_1, w_1〉} \\
  w_3 = v_3 - \cfrac{〈v_3, w_1〉}{〈w_1, w_1〉} w_1
    - \cfrac{〈v_3, w_2〉}{〈w_2, w_2〉}w_2 \\
  w_n = v_n - \cfrac{〈v_n, w_1〉}{〈w_1, w_1〉} w_1
    - \cfrac{〈v_n, w_2〉}{〈w_2, w_2〉}w_2 - \cdots
    - \cfrac{〈v_n, w_{n-1}〉}{〈w_{n-1}, w_{n-1}〉} w_{n-1}
\end{array}
$$

Sea $$ B\:'' $$ una **base ortogonal** en $$ V $$ dado por:

$$u_i = \cfrac{w_i}{\| w_1 \|}, i = 1, 2, \dots, n$$

## Producto cruz

$$a \times b = \| a \|\: \| b \| \sin \theta$$

$$
a \times b =
\begin{vmatrix}
  i & j & k \\
  a_1 & a_2 & a_3 \\
  b_1 & b_{2} & b_{3} \\
\end{vmatrix}
$$
