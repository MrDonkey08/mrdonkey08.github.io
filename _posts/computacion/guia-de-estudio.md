# Sistemas Dígitales

## Sistemas númericos

> [!NOTE]
>
> Al expresar una cantidad, es de vital importancia expresar a qué _sistema numérico_ pertenece, esto para _evitar ambiguedades_. Esto se hace encerrando el número entre parentésis y seguidamente añadiendo la base como subíndice P. ej:

$$
\begin{array}{cc}
(11)_{10},  &  (11)_{2} = (3)_{10}, & (11)_{8} = (9)_{10} & (11)_{8} = (17)_{10}
\end{array}
$$

Un número en _base $r$_ puede ser representado como una _suma de potencias_:

$$A_n ⋅ r^n + A_{n-1} ⋅ r^{n-1} + A_{n-2} ⋅ r^{n-2} + ⋯ + A_{2} ⋅ r^{2} + A_{1} ⋅ r^{1} + A_{0} ⋅ r^{0} + A_{-1} ⋅ r^{-1} + ⋯ + A_{n} ⋅ r^{-n} \tag{1}$$

donde $n$ es la posición del dígito, $A_k$ es el coeficiente, y $r$ es la base a la que pertenece.

### Tabla de equivalencias

| Decimal (Base 10) | Binario (Base 2) | Octal (Base 8) | Hecadecimal (Base 16) |
| ----------------- | ---------------- | -------------- | --------------------- |
| 0                 | 0                | 0              | 0                     |
| 1                 | 1                | 1              | 1                     |
| 2                 | 10               | 2              | 2                     |
| 3                 | 11               | 3              | 3                     |
| 4                 | 100              | 4              | 4                     |
| 5                 | 101              | 5              | 5                     |
| 6                 | 110              | 6              | 6                     |
| 7                 | 111              | 7              | 7                     |
| 8                 | 1000             | 10             | 8                     |
| 9                 | 1001             | 11             | 9                     |
| 10                | 1010             | 12             | A                     |
| 11                | 1011             | 13             | B                     |
| 12                | 1100             | 14             | C                     |
| 13                | 1101             | 15             | D                     |
| 14                | 1110             | 16             | E                     |
| 15                | 1111             | 17             | F                     |

<div style="page-break-after: always;"></div>

### Conversiones

#### Binario, Octal y Hexadecimal a Decimal

1. Representa el número dado en la forma $(1)$.
2. Suma cada uno de los términos siguiendo las reglas de la suma decimal.

#### Decimal a Binario, Octal y Hexadecimal

- **Número decimal entero**: Se divide el número entre base $r$ a convertir, dejando el _cociente entero_; después se divide repetidamente el _coeficiente_ (de la división anterior) entre la _base $r$_ hasta que se convierta en 0. El _primer residuo_ se convierte en el _dígito menos signicante_, mientras que el _ultimo_ el _más significante_.

- **Número decimal fraccional:** Se multiplica el número repetidamente por la _base $r$_, de manera que, en cada multiplicación, se reste la parte entera, hasta que la parte decimal se convierta en $0$. El _primer entero_ es el _dígito menos significante_ y el _último_ el _más significante_

- **Número decimal mixto (entero y fraccional):** Se trabaja la _parte entera_ y la _parte decimal_ por separado, como se indica en los puntos anteriores, y, una vez conseguidas las conversiones a dicha _base $r$_, se suman.

> [!WARNING]
>
> En ocasiones, al convertir un _número decimal fraccional_ a otra base, la parte _fraccional_ u ocupa muchas multiplicaciones para convertirse a 0 o nunca lo será. En estos casos es necesario _truncar_ en algun punto.

#### Binario, Octal y Hexadecimal

> [!IMPORTANT]
>
> Como $2³ = 8$ y $2^4 = 16$, entonces tenemos que cada _dígito octal_ corresponde a tres en _binario_ y cada _dígito hexadecimal_ corresponde a cuatro en _binario_.

- **Binario a octal o hexadicimal:** De derecha a izquierda se agrupan sus dígitos (tres en octal y cuatro en hexadecimal), después se convierte cada agrupación en un dígito de la _base a convertir_.

- **Octal y hexadecimal a binario:** Se convierte cada dígito del número en _binario_ de derecha a izquierda.

- **Hexadecimal a octal o viceversa**: Primeramente se convierte el número en _binario_, después, se agrupan de derecha a izquierda (en tres si se quiere convertir a octal y en cuatro a hexadecimal), por último, se convierte cada agrupación de _binario_ a un dígito de la base a convertir.

<!--
## Operaciones en los Sistemas numéricos

> [!NOTE]
>
> Practicamente las _operaciones aritméticas_ (i.e. suma, resta, multiplicación y división) tienen los mismos principios que los de _base_ 10. Por lo tanto haré una explicación general.

### Suma

Al sumar dos o más números en _base r_, lo que hacemos es sumar de derecha a izquierda cada uno de los dígitos de los números; si al sumar los dígitos (de una columna) dan un número de 2 cifras, la cifra significativa (la de la izquierda) se acarrea.

-->

<div style="page-break-after: always;"></div>

## Álgebra de Boole

### Axiomas

|  N  | Axioma    |             Suma             |        Multiplicación        |
| :-: | --------- | :--------------------------: | :--------------------------: |
|  1  | Identidad |         $0 + 0 = 0$          |       $0 \cdot 0 = 0$        |
|  2  | Identidad |         $1 + 1 = 1$          |       $1 \cdot 1 = 1$        |
|  3  | -         | $0 \cdot 1 = 0 \cdot 1 = 0$  |     $1 + 0 = 0 + 1 = 1$      |
|  4  | Negación  | $A = 0 \to \overline{A} = 1$ | $A = 1 \to \overline{A} = 0$ |

### Teoremas

#### Una variable

|  N  | Leyes           |              Suma               |                      Multiplicación                       |
| :-: | --------------- | :-----------------------------: | :-------------------------------------------------------: |
|  1  | Identidad       |           $A + A = A$           |                        $A ⋅ A = A$                        |
|  2  | Elemento Neutro |           $0 + A = A$           |                        $1 ⋅ A = A$                        |
|  3  | Negación        | $(\overline{A}) = \overline{A}$ | $\overline{(\overline{A})} = \overline{\overline{A}} = A$ |
|  4  | -               |           $1 + A = 1$           |                        $0 ⋅ A = 0$                        |
|  5  | -               |     $A + \overline{A} = 1$      |                  $A ⋅ \overline{A} = 0$                   |

#### Dos variables

|  N  | Leyes         |                                 Suma                                  |                         Multiplicación                         |
| :-: | ------------- | :-------------------------------------------------------------------: | :------------------------------------------------------------: |
|  1  | Conmutativa   |                            $A + B = B + A$                            |                        $A ⋅ B = B ⋅ A$                         |
|  2  | Redundancia   |                           $A + (A ⋅ B) = A$                           |                       $A ⋅ (A + B) = A$                        |
|  3  | Combinación   |                   $(A ⋅ B) + A ⋅ \overline{B} = A$                    |                $(A + B)(A + \overline{B}) = A$                 |
|  4  | DeMorgan      |           $\overline{A + B} = \overline{A} ⋅ \overline{B}$            |        $\overline{A ⋅ B} = \overline{A} + \overline{B}$        |
|  5  | Absorción     |                   $A + (\overline{A} ⋅ B) = A + B$                    |                $A ⋅ (\overline{A} + B) = A ⋅ B$                |
|  6  | OR Exclusiva  |      $A \oplus B = A \cdot \overline{B} + \overline{A} \cdot B$       |      $A \oplus B = (A + B)(\overline{A} + \overline{B})$       |
|  7  | XOR Exclusiva | $\overline{A \oplus B} = A \cdot B + \overline{A} \cdot \overline{B}$ | $\overline{A \oplus B} = (A + \overline{B})(\overline{A} + B)$ |

#### Tres variables

|  N  | Leyes        |                               Suma                                |                         Multiplicación                         |
| :-: | ------------ | :---------------------------------------------------------------: | :------------------------------------------------------------: |
|  1  | Asociativa   |                    $(A + B) + C = A +(B + C)$                     |                   $(A ⋅ B) ⋅ C = A ⋅(B ⋅ C)$                   |
|  2  | Distributiva |                   $A + (B ⋅ C) = A ⋅ B + A ⋅ C$                   |                 $A ⋅ (B + C) = (A + B)(A + C)$                 |
|  3  | Consenso     | $A ⋅ B + \overline{A} ⋅ C + A \cdot B = A ⋅ B + \overline{A} ⋅ C$ | $(A + B)(\overline{A} + B)(B + C) = (A + B)(\overline{A} + C)$ |
