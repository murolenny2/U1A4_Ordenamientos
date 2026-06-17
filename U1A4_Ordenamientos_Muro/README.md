# U1A4 - Evaluación de Métodos de Ordenamiento

## 1. Introducción

En esta práctica se implementaron y evaluaron dos algoritmos clásicos de ordenamiento: Bubble Sort y QuickSort. El objetivo principal fue analizar su desempeño mediante pruebas controladas en Python, comparando sus tiempos de ejecución bajo diferentes tamaños de entrada.

El análisis experimental permitió relacionar los resultados obtenidos con la complejidad teórica de cada algoritmo.

---

## 2. Objetivo

Implementar los algoritmos Bubble Sort y QuickSort en Python y evaluar su rendimiento utilizando diferentes tamaños de datos, realizando múltiples repeticiones para obtener resultados estadísticamente representativos.

---

## 3. Metodología

Se desarrolló el programa en Python utilizando Visual Studio Code como entorno de desarrollo.

Se consideraron los siguientes tamaños de entrada:

- 100 elementos
- 1000 elementos
- 5000 elementos
- 10000 elementos

Para cada tamaño se evaluaron dos escenarios:

- Lista aleatoria
- Lista invertida

Se realizaron 5 repeticiones por cada combinación de algoritmo y tipo de lista.

Para la medición del tiempo de ejecución se utilizó la biblioteca `timeit`, y para la organización de resultados se empleó `pandas`.

Se calcularon:

- Tiempo promedio
- Desviación estándar

Los resultados fueron exportados en formato CSV y Excel.

---

## 4. Resultados

### 4.1 Lista Aleatoria (Tiempo Promedio en segundos)

| Tamaño | Bubble Sort | QuickSort |
|--------|-------------|-----------|
| 100    | 0.00042984  | 0.0000671 |
| 1000   | 0.03214292  | 0.00090948 |
| 5000   | 0.82571382  | 0.00688954 |
| 10000  | 3.4371196   | 0.0168524 |

### 4.2 Análisis Gráfico

La gráfica comparativa muestra claramente que el tiempo de ejecución de Bubble Sort crece de manera acelerada conforme aumenta el tamaño de la entrada, mientras que QuickSort mantiene un crecimiento significativamente menor.

![Gráfica Comparativa](Evidencia/grafica_comparativa.png)

---

## 5. Análisis

Los resultados experimentales confirman la complejidad teórica de cada algoritmo:

- Bubble Sort: O(n²)
- QuickSort (promedio): O(n log n)

Se observa que a medida que el tamaño del conjunto de datos aumenta, la diferencia en el tiempo de ejecución entre ambos algoritmos se vuelve considerablemente mayor.

Para aplicaciones que requieren procesamiento eficiente de grandes volúmenes de datos, QuickSort representa una alternativa significativamente más adecuada.

---

## 6. Estructura del Proyecto
