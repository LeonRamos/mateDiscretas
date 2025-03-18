
# Representación de los grafos

La representación de los grafos es fundamental tanto en matemáticas como en computación. En este capítulo, exploraremos cómo se representan los grafos desde ambas perspectivas, proporcionando ejemplos prácticos para cada una.

## 5.2.1 Representación matemática

En matemáticas, los grafos se pueden representar mediante matrices y listas. A continuación, se presentan tres ejemplos de representación matemática:

### Ejemplo 1: Matriz de adyacencia
La matriz de adyacencia es una forma común de representar grafos. Para un grafo con \( n \) vértices, se crea una matriz \( n \times n \) donde la entrada \( (i, j) \) es 1 si existe una arista entre los vértices \( i \) y \( j \), y 0 en caso contrario. Para grafos no dirigidos, la matriz es simétrica.

**Ejemplo de matriz de adyacencia para un grafo no dirigido:**

Supongamos un grafo con vértices \( A, B, C \) donde \( A \) está conectado a \( B \) y \( C \), y \( B \) está conectado a \( C \). La matriz de adyacencia sería:

\[
\begin{pmatrix}
0 & 1 & 1 \\
1 & 0 & 1 \\
1 & 1 & 0
\end{pmatrix}
\]

### Ejemplo 2: Matriz de incidencia
La matriz de incidencia se utiliza para representar la relación entre vértices y aristas. Cada fila representa un vértice y cada columna una arista. La entrada \( (i, j) \) es 1 si el vértice \( i \) está conectado por la arista \( j \), y 0 en caso contrario.

**Ejemplo de matriz de incidencia:**

Para el mismo grafo anterior, supongamos que las aristas son \( AB, AC, BC \). La matriz de incidencia sería:

\[
\begin{pmatrix}
1 & 1 & 0 \\
1 & 0 & 1 \\
0 & 1 & 1
\end{pmatrix}
\]

### Ejemplo 3: Lista de adyacencia
La lista de adyacencia es una forma eficiente de representar grafos, especialmente cuando son dispersos. Cada vértice se asocia con una lista de sus vértices adyacentes.

**Ejemplo de lista de adyacencia:**

Para el grafo anterior, la lista de adyacencia sería:
- \( A: [B, C] \)
- \( B: [A, C] \)
- \( C: [A, B] \)

## 5.2.2 Representación computacional

En computación, los grafos se pueden representar mediante estructuras de datos como matrices y listas. A continuación, se presentan tres ejemplos de representación computacional paso a paso:

### Ejemplo 1: Implementación de matriz de adyacencia en Python

```
import numpy as np

# Definir la matriz de adyacencia para un grafo no dirigido
matriz_adyacencia = np.array([,,
])

# Mostrar la matriz
print(matriz_adyacencia)
```

### Ejemplo 2: Implementación de matriz de incidencia en Python

```
import numpy as np

# Definir la matriz de incidencia
matriz_incidencia = np.array([,,
])

# Mostrar la matriz
print(matriz_incidencia)
```

### Ejemplo 3: Implementación de lista de adyacencia en Python

```
# Definir la lista de adyacencia
lista_adyacencia = {
    'A': ['B', 'C'],
    'B': ['A', 'C'],
    'C': ['A', 'B']
}

# Mostrar la lista
for vertice, adyacentes in lista_adyacencia.items():
    print(f"{vertice}: {adyacentes}")
```

