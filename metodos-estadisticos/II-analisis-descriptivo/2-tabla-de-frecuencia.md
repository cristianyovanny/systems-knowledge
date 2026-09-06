## Tablas de frecuencia

Las **tablas de frecuencia** son una herramienta que permite **organizar y resumir los datos**, mostrando cómo se distribuyen los valores de una variable y facilitando su interpretación.

### Uso principal

Las tablas de frecuencia se utilizan para:

* **Describir variables cualitativas y cuantitativas discretas.**
* **Identificar patrones, concentraciones o valores frecuentes** dentro de los datos.
* Servir como **base para la construcción de gráficos**, como gráficos de barras, gráficos circulares o histogramas, según el tipo de variable.

---

## Principales medidas de frecuencia

### 1. Frecuencia absoluta ($f_i$)

Es el **número de veces que aparece un determinado valor o categoría** dentro del conjunto de datos.

$$
f_i = \text{Número de ocurrencias del valor } i
$$

### 2. Frecuencia relativa ($h_i$)

Es la **proporción de observaciones que corresponde a un determinado valor o categoría respecto al total de observaciones**.

$$
h_i = \frac{f_i}{N}
$$

Donde:

* $f_i$ = frecuencia absoluta.
* $N$ = número total de observaciones.

### 3. Porcentaje (%)

Es la **frecuencia relativa expresada como porcentaje**.

$$
\% = h_i \times 100
$$

---

# Tablas de frecuencia para variables categóricas

Supongamos que encuestamos a **20 estudiantes de ingeniería** sobre su nivel de satisfacción con el laboratorio de manufactura.

**Variable:** Satisfacción  
**Tipo:** Cualitativa ordinal  
**Valores posibles:** Baja, Media, Alta  
**Tamaño de la muestra:** $N = 20$

Datos observados:

* Baja: 3 estudiantes.
* Media: 7 estudiantes.
* Alta: 10 estudiantes.

La tabla de frecuencia sería:

| Satisfacción | Frecuencia absoluta ($f_i$) | Frecuencia relativa ($h_i$) | Porcentaje | Frecuencia acumulada ($F_i$) | Frecuencia relaiva acumulada ($H_i$)
|---|---:|---:|---:|---:|---:|
| Baja | 3 | 0.15 | 15% | 3 | 0.15 |
| Media | 7 | 0.35 | 35% | 10 | 0.50 |
| Alta | 10 | 0.50 | 50% | 20 | 1.00
| **Total** | **20** | **1.00** | **100%** | **—** | **—** |

### Interpretación

* **3 estudiantes (15%)** presentan un nivel de satisfacción bajo.
* **7 estudiantes (35%)** presentan un nivel de satisfacción medio.
* **10 estudiantes (50%)** presentan un nivel de satisfacción alto.

La categoría con mayor frecuencia es **Alta**, con 10 estudiantes, equivalente al **50% de la muestra**.

---

# Tablas de frecuencia para variables continuas

Cuando una variable cuantitativa continua puede tomar una gran cantidad de valores diferentes, una tabla de frecuencia puede construirse **agrupando los datos en intervalos o clases**.

Supongamos que se obtienen **$N = 150$ medidas de la longitud del sépalo** de tres especies de flores Iris.

**Variable:** `sepal_length`  
**Tipo:** Cuantitativa continua  
**Rango de valores observados:** aproximadamente entre **4.3 cm y 7.9 cm**.

En lugar de crear una fila para cada valor observado, se dividen los datos en **$k$ clases o intervalos**.

## Regla de Sturges

Una forma de estimar el número de clases es utilizar la **regla de Sturges**:

$$
k = 1 + 3.322\log_{10}(N)
$$

Donde:

* $N$ = número de observaciones.
* $k$ = número aproximado de clases.

Para $N = 150$:

$$
k = 1 + 3.322\log_{10}(150)
$$

$$
k \approx 8.23
$$

Como el número de clases debe ser entero, se puede utilizar:

$$
k \approx 8
$$

---

## Amplitud o ancho de clase

Una vez determinado el número de clases, se puede calcular el ancho aproximado de cada intervalo:

$$
A = \frac{X_{\max}-X_{\min}}{k}
$$

Donde:

* $A$ = amplitud o ancho de clase.
* $X_{\max}$ = valor máximo observado.
* $X_{\min}$ = valor mínimo observado.
* $k$ = número de clases.

En este caso:

$$
A = \frac{7.9-4.3}{8}
$$

$$
A = 0.45
$$

Por lo tanto, se pueden construir intervalos con un ancho aproximado de **0.45 cm**, por ejemplo:

$$
[4.30,4.75)
$$

$$
[4.75,5.20)
$$

$$
[5.20,5.65)
$$

y así sucesivamente hasta cubrir todo el rango de los datos.

El símbolo **[** indica que el extremo izquierdo está incluido, mientras que **)** indica que el extremo derecho no está incluido.


| Clase (intervalo) | Marca de clase (\(x_i\)) | Frecuencia absoluta (\(f_i\)) | Frecuencia relativa (\(h_i\)) | Frecuencia porcentual (%) | Frecuencia acumulada (\(F_i\)) |
| ----------------- | -----------------------: | ----------------------------: | ----------------------------: | ------------------------: | -----------------------------: |
| [4.3 – 4.75)      |                    4.525 |                            11 |                         0.073 |                      7.3% |                             11 |
| [4.75 – 5.20)     |                    4.975 |                            18 |                         0.120 |                     12.0% |                             29 |
| [5.20 – 5.65)     |                    5.425 |                            27 |                         0.180 |                     18.0% |                             56 |
| [5.65 – 6.10)     |                    5.875 |                            35 |                         0.233 |                     23.3% |                             91 |
| [6.10 – 6.55)     |                    6.325 |                            29 |                         0.193 |                     19.3% |                            120 |
| [6.55 – 7.00)     |                    6.775 |                            18 |                         0.120 |                     12.0% |                            138 |
| [7.00 – 7.45)     |                    7.225 |                             9 |                         0.060 |                      6.0% |                            147 |
| [7.45 – 7.90)     |                    7.675 |                             3 |                         0.020 |                      2.0% |                            150 |
| **Total**         |                    **—** |                       **150** |                     **1.000** |                  **100%** |                          **—** |

---

### Relación con R

En R, estas tablas pueden construirse de diferentes maneras dependiendo del tipo de variable. Para variables categóricas y discretas, una función fundamental es:

```r
c()
data.frame()
str()
as.factor() y factor()
ordered = TRUE
table() y cut()
```

Aprenderemos a cargar datos de forma local (desde el PC) y desde la web, usando las librerías y funciones:

```r
readxl y stringr
read.csv() y read_excel()
str_split_1() y paste0()
```