---
layout: post
title: Sistemas Numéricos
author: Alan Yahir Juárez Rubio

categories:
  - computacion
tags:
  - binario
  - decimal
  - hexadecimal
  - octal
  - permutacion
  - bit
  - byte

date: 2024-06-03 23:08:21

toc:
  sidebar: right
---

Se le llama **sistema numérico** al conjunto de símbolos y reglas que se
combinan para representar cantidades numéricas.

Un _sistema numérico_ está conformado por:

- **Base**: Cantidad de unidades o símbolos con las que cuenta para formar un
  dígito.

- **Numerales**: Conjunto de símbolos con los que se representarán los números.

- **Normas de combinación**: Conjunto de reglas para formas números. A cada
  cifra se le asocian dos propiedades:

  - **Valor intrínseco absoluto**: Valor del dígito sin importar la posición.
  - **Valor posicional o relativo**: Valor del dígito dependiendo.

Para determinar el valor posicional basta multiplicar el valor absoluto por la
base elevada a la posición

Sea

- $$ A $$ el valor absoluto
- $$ P $$ el valor posicional
- $$ n $$ la base

entonces:

$$A \cdot P^n$$

### Notación

Cuando estamos trabajando con diferentes _sistemas numéricos_, es posible que
dos cantidades diferentes se expresen de la misma manera en alguno _sistemas
numéricos_. Para evitar confusiones es importante escribir el como subíndice
la base del sistema numérico, p. ej:

$$
\begin{array}{c}
  \text{Número} && \text{Equivalencia en Decimal} && \text{Sistema Numérico} \\
  1011_{(2)}    && 11_{10}                        && \text{binario} \\
  1011_{(8)}    && 521_{10}                       && \text{octal} \\
  1011_{(10)}   && 1011_{10}                      && \text{decimal} \\
  1011_{(16)}   && 4113_{10}                      && \text{hexadecimal} \\
\end{array}
$$

## Decimal

Es **sistema decimal** es el _sistema numérico_ con el que todos estamos
familizarizados. Conformado por los dígitos 0, 1, 2, 3, 4, 5, 6, 7, 8 y 9.

## Binario

El **sistema binario** es el _sistema numérico_ que es utilizado por la
computación. Conformado por los dígitos 0 y 1.

En la computación el 0 representa ausencia de corriente y 1 paso de corriente.

<div align="center">
  <figure>
    <img
      src="https://static.platzi.com/media/user_upload/Imagen2-11a06d4c-ca67-4d2d-ad60-d3e5655eb79c.jpg"
      alt="Sistema Binario"
      width="400px"
    >
    <figcaption>Fig. 1 Representación de un Flujo de Corriente.</figcaption>
  </figure>
</div>

Con estos estados es posible codificar cualquier cosa, colores, sonidos, texto,
imágenes, videos, etc. P. ej:

- Un color RGB tal como: (73, 16, 119) su equivalente en binario (número con el
  que trabaja el ordenador) sería (0100 1001, 0001 0000, 0111 0111).

> ##### IMPORTANTE
>
> Nótese que se agregaron ceros a la izquierda para completar números de 8
> dígitos, esto porque el computador trabaja con bytes, conjuntos de 8 bits, de 8
> dígitos. Adicionalmente se separaron en grupos de 4 para un mejor apreciación.
{: .block-warning }

## Octal

El _sistema octal_ es el _sistema numérico_ que permite representar cantidades
binarias de una manera más legible. Está conformado por los dígitos del 0 al 7.

Este sistema es utilzado en informática principalmente para abreviar números
binarios. Este sistema no es muy utilizado debido a que es inclusive
inferior al decimal. Para representar números binario grandes es más óptimo
utilizar el hexadecimal.

Existen diferentes notaciones para representar números octales. Una de las más
comúnes consiste en agregar $0x$ después del número octal, p. ej:

$$327164150x$$

## Hexadecimal

EL **sistema hexadecimal** es el _sistema numérico_ utlizado para hacer más
legibles números inmensamente grandes. Está compuesto por los dígitos del 0 al
9 y las letras de la A a la F (en mayúsculas).

En la computación, el _sistema hexadecimal_ es utilizado para los registros
de memorias, para identificar y operar con cada uno de los registros al acceder
a su dirección de memoria, representada por un número hexadecimal.

Existen diferentes notaciones para representar números hexadicimales, para la
manipulación de direcciones de memoria se utiliza el prefijo $0x$. p. ej:

$$0x3F5000AC$$

<div style="page-break-after: always;"></div>

---

# Referencias

- Ohnsonbaugh, R.
  (2005).
  5.2 Representaciones de enteros y algoritmos enteros.
  _Matemáticas Discretas_
  (6ta edición).
  Editorial Pearson.

- hiru.eus
  (s.f.).
  _Sistemas De Numeración_
  Recuperado el 03 de junio de 2024 de
  <https://www.hiru.eus/es/matematicas/sistemas-de-numeracion>

- Ok diario
  (agosto 29, 2023).
  _Qué es el sistema hexadecimal, para qué sirve y ejemplos_.
  Recuperado el 03 de junio de 2024 de
  <https://okdiario.com/curiosidades/como-funciona-sistema-hexadecimal-3556445>

- nzaratep
  (febrero 21, 2023).
  _Sistema Octal_.
  Recuperado el 03 de junio de 2024 de
  <https://niixer.com/index.php/2023/02/21/sistema-numerico-octal/>
