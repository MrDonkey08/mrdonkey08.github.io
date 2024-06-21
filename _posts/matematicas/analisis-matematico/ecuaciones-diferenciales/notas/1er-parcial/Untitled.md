---
title: 13-02-2023
author: Alan Yahir Juárez Rubio

teacher: Husai

aliases:
tags: matematicas, ecuaciones-diferenciales,

creation date: 13-02-2023
last modification date: 13-02-2023

type: Apuntes de clase
---

---

#

La forma estándar de una ecuacion diferencial ordinari lineal de orden 1 es $y\: '+ P(x)y= Q(x)$ donde $P$ y $Q$ únicamente dependen de $x$

> [!NOTE]
>
> $$\cfrac{d}{dx} \left[e^{\int P(x)dx} \right] $$

---

#### Ejemplos

Determina la solución general de

1. $$4y\: ' - 8y + 7 = 0$$

Llevar ecuación a forma estándar

De lado izquierdo el lado izquierdo a la incógnita y las que no la incluyen del lado derecho:

$$
\begin{array}{l}
4y\: -8y = -7 \\
y\: \frac{-8y = -7}{4}\\
\end{array}
$$

$P(x) = -2$
$Q(x)$

$$
\begin{array}{l}
\mu(x) = e^{\int P(x)dx} = e^{-2x}\\
e^{- \int P(x)dx} = e^{2x}
\end{array}
$$

$$
\begin{array}{l}\mu(x)Q(x)dx
= -\frac{7}{4} \left( \frac{1}{2} \right) \int -e^{-2x}dx
= \frac{7}{8} \int e^udu
\end{array}
$$

La solución general es:

$$
\begin{array}{l}
y = e^{2x} \left[{\frac{7}{8}} e^{-2x} + c \right]
\end{array} \\
y = \frac{7}{8} + ce^{2x}


$$

$$
\begin{array}{l}
xy\:' - (4y + 6x^6 e^x) = 0\\
xy\:' -4y = x^6 e^x\\
\text{Se divide todo entre x}\\
y\:' - \frac{4}{x} y = x^5 e^5
\end{array}
$$

$$
\begin{array}{ll}
P(x) = -\frac{4}{x}, & Q(x) = x^5 e^x
\end{array}
$$

Por fórmula

Logaritmo natural de x

$$
\begin{array}{l}
\int P(x)dx
= \int - \frac{4}{x}
= -4 \ln |x|
\\
\mu(x) = e^{- \int P(x)dx}
= e^{-4 \ln |x|
= e^{\ln (|x|^-4)}
= |x|^{-4}
= |x^{-4}|
= x^{-4}
}
\end{array}
$$

$$
\begin{array}{l}
\int x^{-4} x^5 e^xdx
= \int x e^x dx
\end{array}
$$

<!-- Integración por tabulación -->

| signo | $u$ | $dv$  |
| ----- | --- | ----- |
| +     | $x$ | $e^x$ |
| -     | 1   | $e^x$ |
| +     | 0   | $e^x$ |

$$
\begin{array}{l}
xe^x - e^x
= (x-1) e^x
\end{array}
$$

Solución general

$$
\begin{array}{l}
y = x^4[(x-1)e^x + c]
\end{array}
$$

---

3. $$
   \begin{array}{l}
   \cos (\theta) \cfrac{dr}{d\theta} + r - \cos^2(\theta = 0\\ \\
   \text{Forma estándar}\\ \\
   \cos (\theta) \cfrac{dr}{d\theta} + r
   = \cos^2(\theta \\
   \frac{dr}{d\theta} + \frac{1}{\cos (\theta)}r = \cos(\theta)
   \end{array}
   $$
   $$
   \begin{array}{ll}
   P(\theta) = \frac{1}{\cos(\theta)}
   = \sec(\theta)\\
   Q(\theta) = \cos\theta
   \end{array}
   $$

$$
\begin{array}{l}
\int P(\theta) d\theta
= \int \sec (\theta) dx = \ln [sec(\theta) + \tan]
\\
\mu(\theta) = e^{-\int P(\theta)d \theta}
= e^{\ln[\sec (\theta) + \tan(\theta)]^{-1}}
=\sec(\theta) + \tan(\theta) \\
e^{-\int P(\theta)d\theta}
= e^{ln}
\end{array}
$$

---

## Referencias

- Notas de clase.
