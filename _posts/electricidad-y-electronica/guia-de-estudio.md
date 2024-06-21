---
title: Circuitos electrónicos y electromagnetismo
author: Alan Yahir Juárez Rubio

aliases: circuitos, electronica, electromagnetismo
tags: formulario/circuitos, glosario/circuitos

creation date: 14-03-2023
last modification date: 15-03-2023

type: Formulario, Guía de Estudio
---

# Guía de estudio: Circuitos electrónicos y electromagnetismo

## Ley de ohm

| Nombre                                      | Concepto                   | Símbolo |  Equivalencia  |     Unidad      | Símbolo de unidad |
| :------------------------------------------ | :------------------------- | :-----: | :------------: | :-------------: | :---------------: |
| Voltaje / Tensión / Diferencia de potencial | Fuerza / Impulso del flujo |   $V$   |   $R\cdot I$   |  volt / voltio  |        $V$        |
| Resistencia                                 | Resistencia del flujo      |   $R$   | $\cfrac{V}{I}$ |   ohm / ohmio   |      $\ohm$       |
| Intensidad / Corriente /                    | Rapidez del flujo          |   $I$   | $\cfrac{V}{R}$ | amper / amperio |        $A$        |

## Código de cólores para resistencias

En la actualidad, las **resistencias** vienen con un **código de colores** para indicar su **valor**. Este código consta de 3, 4, 5 o hasta 6 franjas, siendo 4 el más común.

| No. de franjas | Dígito 1 | Dígito 2 | Dígito 3 | Escala | Tolerancia | Coeficiente de temperatura |
| :------------: | :------: | :------: | :------: | :----: | :--------: | :------------------------: |
|       4        |    1     |    2     |    -     |   3    |     4      |             -              |
|       5        |    1     |    2     |    3     |   4    |     5      |             -              |
|       6        |    1     |    2     |    3     |   4    |     5      |             6              |

<br>

| Franjas    | Dígitos |     Escala     | Tolerancia | Coeficiente de temperatura |
| :--------- | :-----: | :------------: | :--------: | :------------------------: |
| Negro      |    0    |       x1       |     -      |         250 ppm/K          |
| Café       |    1    |      x10       |     1%     |         100 ppm/K          |
| Rojo       |    2    |      x100      |     2%     |          50 ppm/K          |
| Naranja    |    3    |     x1,000     |     3%     |          15 ppm/K          |
| Amarillo   |    4    |    x10,000     |     4%     |          25 ppm/K          |
| Verde      |    5    |    x100,000    |    0.5%    |          20 ppm/K          |
| Azul       |    6    |   x1'000,000   |   0.25%    |          10 ppm/K          |
| Violeta    |    7    |  x10'000,000   |    0.1%    |          5 ppm/K           |
| Gris       |    8    |  x100'000,000  |   0.05%    |          1 ppm/K           |
| Blanco     |    9    | x1,000'000,000 |     -      |             -              |
| Dorado     |    -    |      x0.1      |     5%     |             -              |
| Plata      |    -    |     x0.01      |    10%     |             -              |
| Sin franja |    -    |       -        |    20%     |             -              |

Donde:

- El _número_ formado por los **dígitos** se multiplican por la **escala** para obtener el _valor de la resistencia_, el _valor ideal_.
- La **tolerancia** indica cuánto puede variar (tanto por arriba como por debajo) el _valor de la resistencia_.
- El **coeficiente de temperatura** ($\alpha$) indica la _variación del valor de la resistencia_ tomando en cuenta su _temperatura_.

> [!NOTE] Resistencia dependiente de la temperatura
>
> $$R = R_0 \left[1+\alpha \left(T-T_0\right)\right]$$ donde:
>
> - $\alpha =$ **coeficiente de temperatura**
> - $R_0 =$ **Resistencia inicial**, es decir, la que se obtuvo con la temperatura inicial
> - $T_0 =$ **Temperatura inicial**, es decir, la temperatura con la que se obtuvo la **resistencia inicial**
> - $R =$ **Resistencia** tomando en cuenta la temperatura
> - $T =$ **Temperatura** a la que se encuentra la resistencia

## Valor teórico y experimental

En la construcción de circuitos electrónicos nos encontramos con dos tipos de valores:

- **Valor teórico o ideal**: Respecto a los _componentes del circuito_, son aquellos _valores_ que vienen en su diagrama. Los **valores calculados**, (resistencia, amperaje, voltaje, etc.) también son **valores teóricos**.
- **Valor real o experimental**: Son aquellos _valores_ que se encuentran al construir el circuito. Estos _valores_ se encuentran al _medir_ las _magnitudes_ de los _componentes_ y las _magnitudes_ del circuito con herramientas tal como el _amperímetro_, el _voltímetro_, el _ohmímetro_ o el _multímetro_.

### Porcentaje de error

El **porcentaje de error** es una métrica que nos permite saber cuánto error hubo en los _valores_ conseguidos del circuito. Esta métrica se consigue al relacionar los **valores teóricos** con los **valores experimentales** de la siguiente manera:

$$\%\text{error} = \frac{|\text{Valor teórico} - \text{Valor experimental}|}{\text{Valor teórico}} \times 100$$

<!-- <div style="page-break-after: always;"></div>


## Referencias

- https://www.youtube.com/watch?v=ZakHnvGVxLk
- http://hyperphysics.phy-astr.gsu.edu/hbasees/electric/restmp.html
- https://electronics.stackexchange.com/questions/146795/what-does-ppm-k-correspond-to
- https://wikarien.blogspot.com/2016/12/how-to-read-resistor-color-codes.html
- https://es.wikipedia.org/wiki/Codificaci%C3%B3n_de_colores#Resistencias,_condensadores_e_inductores

-->
