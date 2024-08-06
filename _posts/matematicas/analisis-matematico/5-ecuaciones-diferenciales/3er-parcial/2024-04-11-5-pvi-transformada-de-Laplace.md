---
layout: post
title: Problemas de Valor Inicial con la Transformada de Laplace
author: Alan Yahir Juárez Rubio

categories:
  - matematicas
  - ecuaciones-diferenciales
tags:
  - ecuacion-diferencial-lineal
  - principio-de-superposicion

date: 11-04-2023
last_updated: 11-04-2023
---

## Transformada de una Derivada

Si $$ Y(S) = \mathcal{L} \{y\:'(t) \} $$, entonces

$$
\begin{array}{l}
  \mathcal{L} \{y\:'(t)\}    &=& sY(S)     - y(0) \\
  \mathcal{L} \{y\:''(t)\}   &=& s^{2}Y(S) - sY(0)       - y(0)\\
  \mathcal{L} \{y\:'''(t)\}  &=& s^{3}Y(S) - s^{2}Y(0)   - sY(0)  - y(0)\\
  \mathcal{L} \{y^{(n)}(t)\} &=& s^{n}Y(S) - s^{n-1}Y(0) - \cdots - sY^{(n-2)}(0) - y^{(n-2)}(0)\\
\end{array}
$$
