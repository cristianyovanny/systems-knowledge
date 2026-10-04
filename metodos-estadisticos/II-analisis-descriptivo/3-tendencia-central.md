# Medidas de tendencia central

Las **medidas de tendencia central** son medidas estadísticas que permiten identificar un valor que representa, de manera resumida, la **posición central o típica** de un conjunto de datos.

La idea de **“centro”** hace referencia al valor alrededor del cual tienden a concentrarse o distribuirse las obser|vaciones.

Las principales medidas de tendencia central son:

* **Media aritmética**
* **Mediana**
* **Moda**

## Media aritmética

La **media aritmética**, comúnmente llamada **promedio**, se obtiene sumando todos los valores de un conjunto de datos y dividiendo el resultado entre el número total de observaciones.

$$
\bar{x}=\frac{\sum_{i=1}^{n}x_i}{n}
$$

Donde:

* \($\bar{x}$\) = media aritmética.
* \($x_i$\) = valor de la observación \($i$\).
* \($n$\) = número total de observaciones.

**Ventaja:** es fácil de calcular, interpretar y utilizar en diferentes procedimientos estadísticos.

**Desventaja:** puede verse afectada considerablemente por **valores atípicos o extremos**.

## Mediana

La **mediana** es el valor que ocupa la posición central de un conjunto de datos cuando las observaciones se ordenan de menor a mayor.

Su función es dividir los datos ordenados de manera que, aproximadamente, la mitad de las observaciones quede por debajo y la otra mitad por encima.

Primero se ordenan los datos de menor a mayor.

Si \(n\) es impar:

$$
Me=x_{\left(\frac{n+1}{2}\right)}
$$

Si \(n\) es par:

$$
Me=\frac{x_{\left(\frac{n}{2}\right)}+x_{\left(\frac{n}{2}+1\right)}}{2}
$$

**Ventaja:** es poco sensible a valores extremos, por lo que resulta especialmente útil cuando los datos presentan asimetría o valores atípicos.

**Desventaja:** utiliza principalmente la posición de los datos y no considera directamente la magnitud de todas las observaciones, por lo que puede perder información respecto a la media.

## Moda

La **moda** es el valor o categoría que presenta la **mayor frecuencia** dentro de un conjunto de datos.

Se puede expresar como:

$$
Mo=x_k \quad \text{tal que} \quad f_k=\max(f_i)
$$

Donde:

* \($f_i$\) = frecuencia absoluta asociada al valor \($x_i$\).
* \($x_k$\) = valor que presenta la mayor frecuencia.

**Ventaja:** puede utilizarse tanto con datos cuantitativos como con datos cualitativos o categóricos.

**Desventaja:** puede no existir una moda única o puede haber varias modas cuando diferentes valores presentan la misma frecuencia máxima.

## Comparación rápida

| Medida      | Representa            | Sensibilidad a valores extremos                 | Aplicación                                           |
| ----------- | --------------------- | ----------------------------------------------- | ---------------------------------------------------- |
| **Media**   | Promedio de los datos | Alta                                            | Variables cuantitativas                              |
| **Mediana** | Posición central      | Baja                                            | Variables cuantitativas, especialmente con asimetría |
| **Moda**    | Valor más frecuente   | No depende directamente de los valores extremos | Variables cualitativas y cuantitativas               |


---

### Relación con R

Ejemplo de las medidas de tendencias central en R:

```r
dplyr y modeest
mean(), median(), mfv()
na.rm=TRUE y na_rm=TRUE
```
