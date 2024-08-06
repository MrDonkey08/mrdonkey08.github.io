---
layout: post
title: Codificación de Carácteres
author: Alan Yahir Juárez Rubio
description: Funcionamiento de la codificación de carácteres en ASCII y Unicode (UTF).

categories:
  - informatica
tags:
  - codificacion
  - ascii
  - unicode
  - utf

date: 2024-01-08
last_updated: 2024-06-05 16:46:54

toc:
  sidebar: right

featured: true
---

## Conceptos básicos

- **Código:** Conjunto de elementos que, al ser combinados, representan una
  idea, concepto o información. Un código puede ser texto, palabras, dibujos,
  música, videos, etc. (cualquier forma de comunicación).

- **Codificación:** Acción de convertir ideas e infomación en un _código_

- **Decodificación:** Acción de decifrar cualquier _código_, es decir,
  interpretar el _código_.

### Conceptos en Informática

- **Codificación:** Acción de convertir una serie de bits (lenguaje máquina) en
  otro código, en otro formato de información (números, texto, imágenes...).

- **Decodificación:** Proceso opuesto a la _codificación_, es decir, convertir
  _código_ a lenguaje máquina.

- **Esquema de codificación de carácteres** Esquema que establece el cómo se
  convertirán (códificaran) los carácteres en lenguaje máquina.

## ASCII

**ASCII** (American Standard Code for Information Interchange) es un esquema
compuesto de 1 byte. Fue creado para sistemas de 8 bits. El primer bit (bit de
control) es 0 mientras que los 7 bits restantes son utilizados para representar
carácteres (128 carácteres, del 0 al 127).

<div align="">
  <figure>
    <img
      src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/cf/USASCII_code_chart.png/640px-USASCII_code_chart.png"
      alt="Esquma ASCII"
      width="600px">
    <figcaption>Fig. 1: Esquema ASCII</figcaption>
  </figure>
</div>

Existen dos tipos de carácteres:

- **De control (no imprimibles):** Carácteres que sirve para el uso interno del
  computador.

- **Imprimibles:** Carácteres que se imprimen en pantalla, que podemos visualizar.

Los primeros 32 carácteres y el 128 son _carácteres de control_, mientras que
el resto (32 - 127) son _carácteres imprimibles_ del inglés.

### ASCII-Extendido

El **ASCII-Extendido** fue creado principalmente para aquellos idiomas que
requieren símbolos adicionales al inglés. Este utiliza los 8 bits para
representar carácteres (256 carácteres, del 0 - 255). Los primeros 128
carácteres son los carácteres originales de ASCII, mientras que los 128
restantes (128 - 255) depende de la variación de ASCII-Extendido

> ##### NOTA
>
> Para conocer los diferentes esquemas de ASCII-Extendido recomiendo consultar
> [ASCII Code Sets](https://www.ascii-code.com/character-sets)
{: .block-note }

## Unicode

Unicode (Standard character encoding system) fue creado con el propósito de
remplazar a ASCII. En un principio este se conformaba de 16 bits, siendo los
primeros 7 iguales a ASCII (agregando 0's a la izquierda), la cual soportaba
una gran basta cantidad de carácteres

Si bien Unicode agregó muchísimos carácteres, la versión de 16 bits no era
suficiente, por lo que más tarde fue desarrollada la versión de 32 bits,
soportando todos los idiomas e inclusive emojis. Hoy en día Unicode soporta
hasta 149,813 carácteres.

### UTF

**UTF** (Unicode Transformation Format) es un estándar establecido por Unicode
para que cada símbolo solo ocupe la cantidad de bits necesearios (8, 16 o 32),
en vez de que cada símbolo del archivo esté obligado a utilizar 16 o 32 bits.

Si bien se han inventado varias versiones de UTF, actualmente solo existen 3:

- **UTF-8:** Utiliza mínimo 8 bits; comprenden los símbolos de ASCII. Requieremenos
  menos espacio, pero al utilizar símbolos de 16 y 32 bits requiere mayor
  procesamiento.

- **UTF-16:** Utiliza mínimo 16 bits; comprenden los símbolos de la mayoría de
  los idiomas. Al utilizar símbolos de 32 bits requiere mayor procesamiento.

- **UTF-32:** Utiliza mínimo 32 bits. Comprende todos los idiomas, símbolos de
  matemática, física, geometría, música, etc; y emojis.

<div style="page-break-after: always;"></div>

---

## Referencias

- [TeoCom](https://www.youtube.com/@TeoComEc) (mayo 20, 2020).
  CODIFICACIÓN Y DECODIFICACIÓN | Fundamentos de COMUNICACIÓN.
  Consultado el 08 de enero de 2024 de
  <https://www.youtube.com/watch?v=_zphD-F5b5>

- esic (julio, 2023).
  _¿Qué es la codificación de datos?: tipos y ejemplos_.
  Consultado el 08 de enero de 2024 de
  <https://www.esic.edu/rethink/marketing-y-comunicacion/que-es-codificacion-datos-tipos-ejemplos-c>

- [Manik](https://www.youtube.com/@manik3511) (diciembre 06, 2020).
  _¿Cómo funciona la codificación de caracteres? - ASCII / Unicode_.
  Consultado el 08 de enero de 2024 de
  <https://www.youtube.com/watch?v=M_yNoV3c8DY>

- Wikipedia (s. f.). _Unicode_.
  Consultado el 08 de enero de 2024 de
  <https://en.wikipedia.org/wiki/Unicode>

- IBM Documentation (julio 05, 2022).
  _Formatos UTF_.
  Consultado el 08 de enero de 2024 de
  <https://www.ibm.com/docs/es/db2-for-zos/13?topic=unicode-utfs>

<div style="page-break-after: always;"></div>

---

## Recursos Recomendados

- [Códigos Ascii](https://elcodigoascii.com.ar/)

- [Tablas de Ascii](https://www.ascii-code.com/)

- [Ascii: Sets de carácteres](https://www.ascii-code.com/character-sets)
