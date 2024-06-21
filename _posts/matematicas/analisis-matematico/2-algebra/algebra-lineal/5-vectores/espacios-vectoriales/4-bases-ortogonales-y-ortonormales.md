## Bases Ortogonales y Ortonormales

Sea $S$ un **conjunto** en un **espacio vectorial** $V$ con **producto interno**, se llama **ortogonal**, si todo par de vectores en $S$ es **ortogonal**. Si además, cada vector en $S$ es unitario, se denomina **ortonormal**

**Ortogonal:**

$$<v_{i}, v_{j}> = 0, i \pm j$$

**Ortonormal:** **Ortogonal** y

$$
\displaylines{
\| v_{i} \| = 1, &
i = 1, 2, 3, \dots n
}
$$

### Proceso de Ortonormalización de Gram - Schmidt

Sea $B$ una **base** del espacio $V$ con **producto interno**

Sea $B\:'$ una **base ortogonal** en $V$ dado por:

$$
\begin{array}{ll}
w_{1} = v_{1} \\
w_{2} = v_{2} - \cfrac{<v_{2}, w_{1}>}{<w_{1}, w_{1}>} \\
w_{3} = v_{3} - \cfrac{<v_{3}, w_{1}>}{<w_{1}, w_{1}>}w_{1} - \cfrac{<v_{3}, w_{2}>}{<w_{2}, w_{2}>}w_{2} \\
w_{n} = v_{n} - \cfrac{<v_{n}, w_{1}>}{<w_{1}, w_{1}>}w_{1} - \cfrac{<v_{n}, w_{2}>}{<w_{2}, w_{2}>}w_{2} - \cdots - \cfrac{<v_{n}, w_{1}>}{<w_{n-1}, w_{n-1}>}w_{n-1}
\end{array}
$$

Sea $B\:''$ una **base ortogonal** en $V$ dado por:

$$u_{i} = \cfrac{w_{i}}{\| w_{1} \|}, i = 1, 2, \dots, n$$
