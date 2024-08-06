---
layout: post
title: Transformada de Laplace
author: Alan Yahir Juárez Rubio

categories:
  - matematicas
  - ecuaciones-diferenciales
tags:
  - transformada-de-laplace
  - transformada-inversa-de-laplace
  - teorema-de-traslacion

date: 11-04-2023
last_updated: 11-04-2023

toc:
  sidebar: right
---

La transformada de Laplace de una función $$ f = f\left(t \right) $$ se defiine
como:

$$
f\left(s \right)
  = \mathcal{L}\{f\left(t \right)\}\left(s\right)
  = \int_{0}^{\infty} f\left(t \right)e^{-st}\,dt
$$

## Linealidad

Si $$ f $$ y $$ g $$ son funciones, y $$ k $$ es una constante, entonces:

$$
  \mathcal {L}\{f\left(t \right) \pm g\left(t \right)\}
    = \mathcal{L}\{f\left(t \right)\} \pm \mathcal {L}\{g\}
$$

$$\mathcal {L}\{kf\left(t \right)\} = k\mathcal {L}\{f\left(t \right)\}$$

## Linealidad de la Transformada Inversa

Si $$ f $$ y $$ g $$ son funciones, y $$ k $$ es una constante, entonces:

$$
\mathcal {L}^{-1}\{f\left(s \right) \pm g\left(s\right)\}
  = \mathcal{L}^{-1}\{f\left(s \right)\} \pm \mathcal {L}^{-1}\{g\}
$$

$$
\mathcal {L}^{-1}\{kf\left(s \right)\}
  = k\mathcal {L}^{-1}\{f\left(s \right)\}
$$

## Primer Teorema de Traslación

Si $$ G(S) = \mathcal {L}\{g\left(t \right)\} $$ =, entonces se cumplen:

$$\mathcal {L}\{g\left(t \right)e^{at}\} = G\left(s-a \right)$$

$$
\mathcal {L}^{-1} \{G\left(s-a \right)
  = e^{at} g\left(t \right)
  = e^{at}
\mathcal {L}^{-1} \{G\left(s \right)\}
$$
