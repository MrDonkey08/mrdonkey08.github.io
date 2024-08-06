---
layout: post
title: Funciones Compuestas
author: Alan Yahir Juárez Rubio

categories:
  - matematicas
  - calculo
  - funciones
tags:
  - compuesta

date: 2023-01-12 09:00:00
last_updated: 2024-06-04 15:38:44

toc:
  sidebar: right
---

Las **funciones compuestas** son aquellas que se obtienen cuando las funciones
son evaluadas con otras_funciones.

$$f \circ g (x) = f(g (x)) \tag{$f$ de $g$ de $x$}$$

$$g \circ f(x) = g(f(x)) \tag{$g$ de $f$ de $x$}$$

El rango de la función interna debe satisfacer al dominio de la función externa.

## Ejemplos

$$
\begin{array}{l}
  f(x) = \sqrt{x} \\
  g(x) = x + 2
\end{array}
$$

$$
\begin{array}{l}
  f\circ g (x) = f(g (x)) = \sqrt{x + 2} \\
  g\circ f(x) = g(f(x))= \sqrt{x} +  2
\end{array}
$$

---

$$
\begin{array}{l}
  f(x) = x^2 + x \\
  g(x) = 1 - x
\end{array}
$$

$$f\circ (g(x)) = (1-x)^2 - (1-x) = x^2 - 3x + 2$$

$$g\circ (g(x)) = 1 - (x^2-x) - x^2 - x$$

<div style="page-break-after: always;"></div>

---

## Referencias

- [Carrión, M.](https://platzi.com/profes/mcarrion/)
  (22 de noviembre de 2021).
  _Qué son las funciones compuestas_.
  [Curso Básico de Cálculo Diferencial](https://platzi.com/cursos/calculo-diferencial/).
  [Platzi](https://platzi.com/).
  Recuperado el 13 de enero de 2023 de
  <https://platzi.com/new-home/clases/2612-calculo-diferencial/43619-que-son-las-funciones-compuestas/>
