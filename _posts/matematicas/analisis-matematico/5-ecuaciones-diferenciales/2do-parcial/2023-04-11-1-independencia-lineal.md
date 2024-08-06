---
layout: post
title: Independencia lineal
author: Alan Yahir Juárez Rubio

categories:
  - matematicas
  - ecuaciones-diferenciales
tags:
  - independencia-lineal
  - wronskiano

date: 11-04-2023
last_updated: 11-04-2023

toc:
  sidebar: right
---

Definición: Consideremos las funciones $$ f_1, f_2, f_3, \dots, f_n $$.

1. Diremos que estas funciones son **linealmente independientes** si los únicos
   números que satisfacen la ecuación $$ cf_1, cf_2, cf_3, \dots, cf_n = 0 $$
   son los números $$ c_1 = c_2 = c_3 = \dots = c_n = 0 $$.

2. Diremos que estas funciones son **linealmente dependiendes** si no son
   **línealmente independientes**.

3. El **Wronskiano** de $$ f_1, f_2, f_3, \dots, f_n $$ se define como el
   **determinante**.

$$
W \left(f_1, f_2, f_3, \dots, f_n \right) =
\begin{vmatrix}
  f_1           & f_2           & f_3           & \dots  & f_n \\
  f_1\:'        & f_2\:'        & f_3\:'        & \dots  & f_n\:' \\
  f_1\:''       & f_2\:''       & f_3\:''       & \dots  & f_n\:'' \\
  \vdots        & \vdots        & \vdots        & \ddots & \vdots \\
  {f_1}^{(n-1)} & {f_2}^{(n-1)} & {f_3}^{(n-1)} & \dots  & {f_{n}} ^{(n-1)}
\end{vmatrix}
$$

> ##### IMPORTANTE
>
> En Wronskiano:
>
> - Si $$ \mid D \mid = 0 \to $$ sistema **linealmente dependiente**
> - Si $$ \mid D \mid \neq 0 \to $$ sistema **linealmente independiente**
{: .block-important }

> ##### NOTA
>
> El **Wronskiano** se puede aplicar para **sistemas homogéneos** y
> **heterogéneos**
{: .block-note }
