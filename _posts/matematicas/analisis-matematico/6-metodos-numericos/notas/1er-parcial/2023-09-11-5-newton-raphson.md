---
layout: post
title: Método de Newton-Raphson
author: Alan Yahir Juárez Rubio

categories:
  - matematicas
  - metodos-numericos
tags:
  - newton
  - rapshon
  - ecuaciones-no-lineales

date: 2023-09-11
last_updated: 2024-07-24 20:55
---

Es uno de los métodos más conocidos y poderosos para resolver _ecuaciones no
lineales_, ya que es posible encontrar _raíces reales o complejas_, aunque para
estos últimos presentan grandes ventajas ya que, de antemano, se debe conocer
la complejidad de trabajar con ellas.

El método de Newton-Raphson requiere de un solo valor inicial "cercano a la
raíz".

El método iterativo tiene la forma:

$$X_{n+1} = X_n - \cfrac {f(x_n)}{f'(x_n)}$$
