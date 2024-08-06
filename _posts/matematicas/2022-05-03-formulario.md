---
layout: post
title: Formulario Precálculo
author: Alan Yahir Juárez Rubio

categories:
  - matematicas
  - precalculo
tags:
  - guia-de-estudio
  - formulario

date: 2022-05-03
last_updated: 2024-08-05 19:35

toc:
  beginning: true

pretty_table: true
featured: true
---

En este formulario: $$ A, B, C, D, a, b, c, d, p, q, s \in \Bbb R $$ y son
constantes; $$ n, m \in \Bbb{Z} $$ y $$ r \in \Bbb{Z}^+ $$

## Conjunto de Números Reales

### Propiedades de los Números

|                                                               |                   Suma                   |                 Multiplicación                 |
| ------------------------------------------------------------- | :--------------------------------------: | :--------------------------------------------: |
| Ley conmutativa                                               |             $$ a+b = b+a $$              |          $$ a \cdot b = b \cdot a $$           |
| Ley asociativa                                                |         $$ (a+b)+c = a+(b+c) $$          | $$ (a \cdot b) \cdot c = a \cdot(b \cdot c) $$ |
| Elemento Neutro                                               |             $$ a+(0) = a $$              |             $$ a \cdot (1) = a $$              |
| Elemento inverso (recíproco)                                  |             $ a+(-a) = 0 $$              | $$ a \cdot \left(\cfrac {1}{a} \right) = 1 $$  |
| Ley distributiva de la multiplicación con respecto de la suma | $$ (a+b \cdot c = a \cdot c+b \cdot c $$ |                $$ \leftarrow $$                 |

### Fracciones

$$
\begin{align}
  \cfrac {a}{b}   +   \cfrac {c}{b} &= \cfrac {a  +  c}{b}  \tag{Suma con mismo
denominador} \\
  \cfrac {a}{b}   +   \cfrac {c}{d} &= \cfrac {ad + bc}{cd} \tag{Suma con
distinto denominador} \\
  a               +   \cfrac {c}{b} &= \cfrac {ab +  c}{b}  \tag{Suma con
entero y una fracción} \\
  \cfrac {a}{b} \cdot \cfrac {c}{d} &= \cfrac {ac}{bd}      \tag{Multiplicación
de fracciones} \\
  \cfrac {a}{b} \div  \cfrac {c}{d} &= \cfrac {ad}{bc}      \tag{Division de
fracciones (cruzada)} \\
  \cfrac {a}{b} \cdot \cfrac {c}{c} &= \cfrac {a \cdot c}{b \cdot c}
    = \cfrac {a}{b}                                         \tag{Multiplicación
por unidad}
\end{align}
$$

### Desigualdades

$$
\begin{align}
  \text{ Si } a-b = c \to a > b, \;\; \text{ donde } c > 0 \tag{Mayor que} \\
  \text{ Si } a-b = c \to a < b, \;\; \text{ donde } c < 0 \tag{Menor que} \\
\end{align}
$$

### Valor Absoluto

$$
|a| =
\begin{bmatrix}
  a \geq 0 \to |a| &= a \\
  a   <  0 \to |a| &= -a
\end{bmatrix}
$$

### Distancia entre Dos Puntos

$$
\begin{gather*}
  d(A,B) = |b-a| \\
  d(B,A) = |a-b|
\end{gather*}
$$

## Leyes de los Exponentes

| Nombre                                | Ley                                              |
| ------------------------------------- | ------------------------------------------------ |
| **Ley de separación**                 | $$ (\cfrac {a}{b})^n = \cfrac {a^n}{b^n} $$      |
| **Ley de separación**                 | $$ (ab)^n = a^n b^n $$                           |
| **Multiplicación de bases iguales**   | $$ a^n a^m = a^{n+m} $$                          |
| **Potencia de una base con potencia** | $$ (a^n)^m = a^{nm} $$                           |
| **Potencia cero**                     | $$ a^0 = 1 $$                                    |
| **Potencia negativa**                 | $$ a^{-n} = \cfrac {1}{a^n} $$                   |
| **División de bases iguales**         | $$ \cfrac {a^n}{a^m} = a^{n-m} \ (si \ n > m) $$ |
| **División de bases iguales**         | $$ \cfrac {a^n}{a^m} = \cfrac {1}{a^{m-n}} $$    |
| **De reescritura**                    | $$ a^{m/n} = \sqrt [n]{a^m} $$                   |

## Leyes de los Radicales

| Nombre                                    | Ley                                                                 |
| ----------------------------------------- | ------------------------------------------------------------------- |
| **De separación**                         | $$ \sqrt [n]{ab} = \sqrt [n]{a} \sqrt [n]{b} $$                     |
| **De la raíz m_ésima de la raíz n_ésima** | $$ \sqrt [m] {\sqrt[n]{a}} = \sqrt [nm] {a} $$                      |
| **De cancelación**                        | $$ (\sqrt [n]{a})^n = a $$                                          |
| **De cancelación**                        | $$ \sqrt [n]{a^n} = (a^n)^{1/n} = a $$, si $$ n $$ es impar         |
| **De cancelación**                        | $$ \sqrt [n]{a^n} = (a^n)^{1/n} = \mid a \mid $$, si $$ n $$ es par |
| **De reescritura**                        | $$ \sqrt [n]{a^m} = a^{m/n} $$                                      |

> ##### ADVERTENCIA
>
> $$\sqrt [n]{a^n \pm b^n} \neq a \pm b$$
>
> $$\sqrt [n]{a \pm b} \neq a \pm b$$
{: .block-warning }

## Número Imaginario

**Número imaginario**: $$ i = \sqrt{-1} $$

$$
\begin{array}{l}
  i^0 &= 1 \\
  i^1 &= i \\
  i^2 &= -1 \\
  i^3 &= i^2i    &= (-1)i    &= -i \\
  i^4 &= i^2 i^2 &= (-1)(-1) &= 1
\end{array}
$$

**Número complejo**:
$$ z = a+bi \mid a \in \Bbb R \text{ y } bi \in \Bbb I \to z \in \Bbb C $$

## Operaciones con Polinomios

$$
\begin{align}
  ab^n \pm b^n &= b^n(a \pm 1) \tag{Suma y resta (términos semejantes)} \\
  a(b+c)         &= ab + ac      \tag{Multiplicación}
\end{align}
$$

### Productos Notables

| Nombre                      | Expresión       | Equivalencia                              |
| --------------------------- | --------------- | ----------------------------------------  |
| **Diferencia de cuadrados** | $$ a^2 - b^2 $$ | $$ (a-b)(a+b) $$                          |
| **Suma de cubos**           | $$ a^3 + b^3 $$ | $$ (a+b)(a^2 - ab + b^2) $$               |
| **Diferencia de cubos**     | $$ a^3 - b^3 $$ | $$ (a+b)(a^2 + ab + b^2) $$               |
| **Binomio al cuadrado**     | $$ (a+b)^2 $$   | $$ a^2 + 2ab + b^2 $$                     |
| **Binomio al cuadrado**     | $$ (a-b)^2 $$   | $$ a^2 - 2ab + a^2 $$                     |
| **Binomio al cubo**         | $$ (a+b)^3 $$   | $$ a^3 + 3a^2b + 3ab^2 + b^3 $$           |
| **Binomio a la cuarta**     | $$ (a+b)^4 $$   | $$ a^4 + 4a^3b + 6a^2b^2 + 4ab^3 + b^4 $$  |

## Binomio de Newton

$$
(a+b)^n
  = a^n
    + \cfrac {n}{1!}a^{n-1}b
    + \cfrac {n(n-1)}{2!}a^{n-2}b^2
    + \cfrac {n(n-1)(n-2)}{3!}a^{n-3}b^3
    + \cdots + b^n
$$

## K<sub>ésimo</sub> Término

$$
K_{\text{ésimo}} \text{ término }
  = \cfrac
      {n!}
      {(n-r+1)!(r-1)!}
    \cdot a^{n-r+1}
    \cdot b^{r-1}
$$

> ##### NOTA
>
> donde:
>
> - $$ n = $$ potencias.
> - $$ r $$ = número del término a buscar.
> - $$ n,r \in \Bbb{Z}^+ $$.
{: .block-note }

## Factorización

**Por fórmula**: Consultar las fórmulas de productos notables.

**Por término común**: $$ x^2 + ax = x(x+a) $$

**Por agrupación**:

$$
\begin{gather*}
  ax  + bx  + ay  + by \\
  (ax + bx) + (ay + by) \\
  x(a + b)  + y(a + b) \\
  (a + b)(x + y) \\
\end{gather*}
$$

## Operaciones con Números Complejos en Forma Algebraica

$$
\begin{array}{c|c|c}
  \
  \text{Suma y resta} & \text{División} & \text{Multiplicación} \\
  \eqalign {
    z_1 + z_2
      &= (a+bi)+(c+di) \\
      &= (a+c)(b+d)i \\
      \\
    z_1 + z_2
      &= (a+bi) - (c+di) \\
      &= (a-c) + (b-d)i
  }
  & \eqalign {
    \cfrac {z_1}{z_2}
      &= \cfrac {z_1}{z_2} \cdot \cfrac {z_2}{x_2} \\
      &= \cfrac {a + bi}{c + di} \cdot \cfrac {c-di}{c-di} \\
      &= \cfrac {ac + (bc-ad)i-bdi^2}{c^2 d^2 i^2}
  }
  & \eqalign{
    z_1 \cdot z_2
      &= (a + bi)(c + di) \\
      &= ac + bci + adi + bdi^2 \\
      &= ac + (bc + ad) + bdi^2 \\
  }
\end{array}
$$

## Intérvalos y Desigualdades

### Intérvalos

<div align="center">
  <figure>
    <img
      src="/assets/img/precalculo/2024-08-05-intervalos.webp"
      alt="Intérvalos"
      width="600px"
    >
    <figcaption>Fig. 1: Intérvalos</figcaption>
  </figure>
</div>

### Desigualdades

- Si $$ a > b $$ y $$ b > c $$, entonces $$ a > c $$
- Si $$ a > b $$, entonces $$ a+c > b+c $$
- Si $$ a > b $$ y $$ c > 0 $$, entonces $$ ac > bc $$
- Si $$ a > b $$ y $$ c < 0 $$, entonces $$ ac < bc $$

> ##### NOTA
>
> Al multiplicar o dividir ambos lados de una desigualdad por un número real
> negativo, el signo de la desigualdad se invierte.
{: .block-note }

### Desigualdad con Valor Absoluto

| Caso |          Modelo          |           Solución            |
| :--: | :----------------------: | :---------------------------: |
|  1   |  $$ \mid a \mid < b $$   |        $$-b < a < b $$        |
|  2   | $$ \mid a \mid \leq b $$ |     $$-b \leq a \leq b $$     |
|  3   |  $$ \mid a \mid > b $$   |    $$ a < -b \cup a > b $$    |
|  4   | $$ \mid a \mid \geq b $$ | $$ a \leq -b \cup a \geq b $$ |

## Ecuaciones Cuadráticas (de Segundo Grado)

### Completar el Cuadrado

| Expresión original |           Término a sumar           |             Expresión Transformada             |              Equivalencia               |
| :----------------: | :---------------------------------: | :--------------------------------------------: | :-------------------------------------: |
|   $$ x^2 + kx $$   | $$ \left(\cfrac {k}{2} \right)^2 $$ | $$ x^2 + kx + \left(\cfrac {k}{2} \right)^2 $$ | $$ \left(x + \cfrac {k}{2} \right)^2 $$ |
|   $$ x^2 - kx $$   | $$ \left(\cfrac {k}{2} \right)^2 $$ | $$ x^2 - kx + \left(\cfrac {k}{2} \right)^2 $$ | $$ \left(x - \cfrac {k}{2} \right)^2 $$ |

### Fórmula General

$$
\begin{gather*}
x = \cfrac
  {-b \pm \sqrt {b^2 - 4ac}}
  {2a}
  \tag{Para $ ax^2 + bx + c = 0, a \neq 0 $ }
\end{gather*}
$$

#### Discriminante

$$ D = b^2 - 4ac $$

1. $$ D \mid D > 0 \Rightarrow $$ Dos soluciones reales
2. $$ D \mid D < 0 \Rightarrow $$ Dos soluciones complejas
3. $$ D \mid D = 0 \Rightarrow $$ Solución repetida, una única solución

### Método de Po-Shen Loh

$$ ax^2 + bx + c = d $$

Para factorizar esto podemos buscar dos números que multiplicados den $$ c $$
y sumados den $$ b $$. Se puede hacer por prueba y error o aplicando el
**método de Po-shen Lo**:

1. Dividimos toda la expresión entre $$ a $$

$$ x^2 + \cfrac {bx}{a} + \cfrac {c}{a} = \cfrac {d}{a} $$

2. Buscamos dos números que sumados den $$ \cfrac {b}{a} $$, lo más sencillo es
hacer cada uno de estos dos números dos números valgan la mitad de $$ \cfrac
   {b}{a} $$

$$
\begin{gather*}
  p + q = \cfrac {b}{a}, & p = \cfrac {b}{2a}, & q = \cfrac {b}{2a}
\end{gather*}
$$

3. Le sumamos a $$ p $$ una cantidad, pero a $$ q $$ se le resta esa misma
   cantidad para mantener el equilibrio

$$
\begin{gather*}
  \cfrac {b}{2a} + s, & \cfrac {b}{2a} - s
\end{gather*}
$$

4. Buscamos los dos números que multiplicados den $$ \cfrac {a}{c} $$

$$
\begin{gather*}
  \left(\cfrac {b}{2a} + s \right) \left(\cfrac {b}{2a} - s \right)
    = \cfrac {c}{a} \\
  \cfrac {b^2}{4a^2} - s^2
    = \cfrac {c}{a}
\end{gather*}
$$

5. Despejamos respecto a $$ s $$

$$
\begin{gather*}
  s^2 = \cfrac {b^2}{4a^2} - \cfrac {c}{a} \\
  s = \pm \sqrt {\cfrac {b^2 - 4ac}{4a^2}} \\
  s = \pm \cfrac {\sqrt{b^2 - 4ac}}{2a}
\end{gather*}
$$

6. Tomamos el valor de $$ s $$, ya sea el positivo o el negativo.
7. Ahora solo sustituimos $$ s $$

$$
\begin{gather*}
  \cfrac {b}{2a} + \cfrac {\sqrt{b^2 - 4ac}}{2a}, &&
  \cfrac {b}{2a} - \cfrac {\sqrt{b^2 - 4ac}}{2a}
\end{gather*}
$$

Entonces tenemos que

$$
\begin{gather*}
  x^2 + \cfrac {bx}{a} + \cfrac {c}{a} = \cfrac {d}{a} \\
  \left(x
    + \cfrac
      {b + \sqrt{b^2 - 4ac}}
      {2a}
  \right)
  \left(x
    + \cfrac
      {b - \sqrt{b^2 - 4ac}}
      {2a}
  \right)
  = \cfrac {d}{a} \\
\end{gather*}
$$

<!-- Asumiendo que tengamos el caso en el que $$ d = 0 $$, entonces

$$
\begin{gather*}
  (x+p)(x-q) = 0 \\
  x = -p = -\cfrac {b + \sqrt{b^2 - 4ac}}{2a} \\  x = -q = - \cfrac
{b-\sqrt{b^2 - 4ac}}{2a}
\end{gather*}
$$

-->

### Valor Absoluto

$$
\begin{gather*}
  |x| = y \\
  x = \pm y
\end{gather*}
$$

> ##### NOTA
>
> La **raíz cuadrada** de una _variable elevada al cuadrado_ te da su
> **valor absoluto**, a menos que se sepa de antemano que _dicha variable_ es
> _positiva o negativa_.
>
> $$
> \begin{gather*}
>   \sqrt{x^2} = |x| \\
>   \sqrt{x^2} = x, x > 0 \\
>   \sqrt{x^2} = - x, x < 0
> \end{gather*}
> $$
>
{: .block-note }

### Por Agrupación

$$
\begin{gather*}
  x^2 + ax + bx + ba = 0 \\
  x(x+a) + b(x+a) = 0 \\
  (x+a)(x+b) = 0
\end{gather*}
$$

### Teorema del Cero

Un producto que da 0 solo puede ser posible si por lo menos uno de los
_factores_ es 0

**Una variable**:

$$
\begin{gather*}
  (x+a)(x+b) = 0 \\ \\
  \
  \begin{array}{l|l}
    \text{Sol. 1} & \text{Sol. 2} \\
    \
    x+a = 0     & x+b = 0 \\
    x_1 = -a     & x_2 = -b
  \end{array}
\end{gather*}
$$

**Dos variables**

$$
\begin{gather*}
  (x+a)(y+b) = 0 \\ \\
  \
  \begin{array}{l|l}
    x+a = 0 & y+b = 0 \\
    x = -a & y = -b
  \end{array}
\end{gather*}
$$

En este caso puede haber 3 posibles soluciones:

$$
\begin{gather*}
  x = -a, y = c, \tag{donde $ c $ puede tener cualquier valor} \\
  y = -b, x = d, \tag{donde $ d $ puede tener cualquier valor} \\
  x = -a, y = -b \\
\end{gather*}
$$

> ##### RECOMENDACIÓN
>
> Recuerda siempre hacer _comprobación_ de todas las posibles soluciones para
> determinar cuál es la solución que satisface la ecuación.
{: .block-tip }

### Por Sustitución

$$ ax^4 + bx^2 + c = 0 $$

1. Aplicar sustitución para simplicar la ecuación original

$$
\begin{gather*}
  \begin{array}{c|c}
  x^2 = u & x^4 = u^2
  \end{array} \\
  \
  au^2 + bu + c = 0
\end{gather*}
$$

2. Resolver la ecuación
3. Sustituir por los valores originales
4. Comprobación

## Fracciones Parciales

Siendo el grado de $$ f(x) $$ menor que el de $$ g(x) $$, entonces tenemos que

$$
\cfrac {f(x)}{g(x)}
  = F_1 + F_2 + \cdots + F_r
$$

tal que $$ F_k $$ tiene una de las formas:

$$
\cfrac {A}{(ax + b)^n} \\
  \text{ o } \\
\cfrac {A_x + B}{(ax^2 + bx + c)^n}
$$

**Factores lineales distintos**:

$$
\cfrac {f(x)}{(ax + b)(cx + d) \cdots}
  = \cfrac {A}{ax + b} + \cfrac {B}{cx + d} + \dots \tag{1}
$$

**Factores lineales repetidos**:

$$
\cfrac {f(x)}{(ax + b)^n}
  = \cfrac {A}{ax + b}
    + \cfrac {B}{(ax + b)^2}
    + \cdots
  \tag{2}
$$

**Factores cuadráticos distintos**:

$$
\cfrac
    {f(x)}
    {(ax^2 + bx + c)(dx^2 + cx + f)}
  = \cfrac
    {Ax + B}
    {ax^2 + bx + c}
    + \cfrac
      {Cx + D}
      {dx^2 + ex + f}
    + \cdots
\tag{3}
$$

**Factores cuadráticos repetidos**:

$$
\cfrac
    {f(x)}
    {(ax^2 + bx + c)^n}
  = \cfrac
    {Ax + B}
    {ax^2 + bx + c}
    + \cfrac
      {Cx + D}
      {(ax^2 + bx + c)^2}
    + \cdots
\tag{4}
$$

### Procedimiento General

1. Asegurarse que el _grado_ del _numerador_ $$ f(x) $$ sea menor que el del
   _denominador_; de ser el caso contrario, aplicar la _división larga_.
2. Factorizar el denominador en _factorles lineales_ $$ px + q $$ o _factores
   cuadráticos irreducibles_.
3. Multiplicar los númeradores de cada $$ F_k $$ por el _mínimo común
   múltiplo_, es decir, por cada uno de los _factores_, para poder convertir la
   expresión en _líneal_.
4. Igualar la expresión encontrada por el numerador $$ f(x) $$.
5. Convertir la expresión en la forma:

$$
f(x) =
  (a_1A + a_2B + \cdots)x
    + (a_3A
    + a_4B
    + \cdots)x^2
    + \cdots
$$

6. Considerando que $$ f(x) = b_1x + b_2 x^2 + \cdots $$, entonces podemos
   _igualar los coeficientes_ de las _potencias semejantes_.de esta manera
   obtenemos un _sistema de ecuaciones_.
7. Sustituir en las _fracciones parciales_ los valores de $$ A, B, \cdots $$.

#### Factores Lineales no Repetidos

En caso de que todos los factores del denominador sean _lineales no repetidos_
$$ (1) $$, entonces podemos aplicar un método alternativo a partir del paso 4.

1. Sustituir los valores de $$ x $$ que hagan que cada uno de los _factores
   lineales_ se conviertan en 0.
2. Resolver cada caso haciendo las sustituciones necesarias.
3. Sustituir en las _fracciones parciales_ los valores de $$ A, B, \dots $$

<!-- ## 20. Fracciones

21. Teorema del residuo y del factor
22. División sintética
23. Teoremas sobre polinomios
24. Gráficas de polinomios
25.
26. Funciones exponenciales
27. Función Logaritmica
27.1 Propiedades de los logaritmos
27.2 Cómo graficar una función logaritmica
27.3 Propiedades de los logaritmicas
29. Funciones trigonométricas

-->

<div style="page-break-after: always;"></div>

---

## Referencias

- W., E. & A., J.
  (2009).
  _Álgebra y trigonometría con geometría análitica_
  (12<sup>a</sup> ed.).
  En S. R. Cervantes (Ed.),
  Editorial CENGAGE Learning.

- [Standen Math](https://www.youtube.com/@StandenMath).
  (mayo 23, 2022).
  _La mejor manera de resolver una ecuación cuadrática_.
  Recuperado el 22 de abril de 2023 de
  <https://www.youtube.com/watch?v=GFO6FCbSCyo>

<div style="page-break-after: always;"></div>

---

## Recursos Recomendados

- [Formulario EDOI - CUCEI](http://mate.cucei.udg.mx/formularioEDOI.pdf)
