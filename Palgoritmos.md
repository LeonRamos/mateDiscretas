
# Ejercicio para Dijkstra

**Título**: Ruta más corta en una ciudad

**Descripción**: En una ciudad, hay varias estaciones de transporte público conectadas entre sí. Cada conexión tiene un tiempo de viaje asociado. Utiliza el algoritmo de Dijkstra para encontrar la ruta más rápida entre dos estaciones específicas.

**Grafo de ejemplo**:

```python
grafo = {
    'A': {'B': 5, 'C': 3},
    'B': {'A': 5, 'D': 2, 'E': 4},
    'C': {'A': 3, 'F': 1},
    'D': {'B': 2, 'E': 1},
    'E': {'B': 4, 'D': 1, 'F': 3},
    'F': {'C': 1, 'E': 3}
}
```

**Tarea**:
1. Implementa el algoritmo de Dijkstra en Python para encontrar la ruta más rápida entre las estaciones 'A' y 'F'.
2. Explica paso a paso cómo funciona el algoritmo en este contexto.
3. Calcula la complejidad temporal del algoritmo.

**Código base**:

```python
import heapq

def dijkstra(grafo, inicio, fin):
    # Implementación del algoritmo
    pass

grafo = {
    'A': {'B': 5, 'C': 3},
    'B': {'A': 5, 'D': 2, 'E': 4},
    'C': {'A': 3, 'F': 1},
    'D': {'B': 2, 'E': 1},
    'E': {'B': 4, 'D': 1, 'F': 3},
    'F': {'C': 1, 'E': 3}
}

inicio = 'A'
fin = 'F'

# Llamar a la función y mostrar el resultado
```

# Ejercicio para BFS

**Título**: Exploración de una red social

**Descripción**: En una red social, los usuarios están conectados entre sí. Utiliza el algoritmo BFS para encontrar a todos los amigos de un usuario específico hasta una distancia de dos grados.

**Grafo de ejemplo**:

```python
grafo = {
    'Alice': ['Bob', 'Charlie'],
    'Bob': ['Alice', 'Dave', 'Eve'],
    'Charlie': ['Alice', 'Frank'],
    'Dave': ['Bob'],
    'Eve': ['Bob', 'Frank'],
    'Frank': ['Charlie', 'Eve']
}
```

**Tarea**:
1. Implementa el algoritmo BFS en Python para encontrar a todos los amigos de 'Alice' hasta dos grados de distancia.
2. Explica cómo se utiliza la cola en este contexto.
3. Discute las ventajas de usar BFS en este tipo de problemas.

**Código base**:

```python
from collections import deque

def bfs(grafo, inicio, distancia_maxima):
    # Implementación del algoritmo
    pass

grafo = {
    'Alice': ['Bob', 'Charlie'],
    'Bob': ['Alice', 'Dave', 'Eve'],
    'Charlie': ['Alice', 'Frank'],
    'Dave': ['Bob'],
    'Eve': ['Bob', 'Frank'],
    'Frank': ['Charlie', 'Eve']
}

inicio = 'Alice'
distancia_maxima = 2

# Llamar a la función y mostrar el resultado
```

# Ejercicio para DFS

**Título**: Búsqueda en un árbol de directorios

**Descripción**: En un sistema de archivos, los directorios están organizados en forma de árbol. Utiliza el algoritmo DFS para encontrar un archivo específico en este árbol.

**Árbol de ejemplo**:

```python
arbol = {
    'root': ['dir1', 'dir2'],
    'dir1': ['file1', 'dir3'],
    'dir2': ['file2'],
    'dir3': ['file3']
}
```

**Tarea**:
1. Implementa el algoritmo DFS en Python para encontrar el archivo 'file3' en el árbol.
2. Explica cómo se utiliza la recursividad o una pila en este contexto.
3. Discute las diferencias entre DFS y BFS en este tipo de problemas.

**Código base**:

```python
def dfs(arbol, inicio, objetivo):
    # Implementación del algoritmo
    pass

arbol = {
    'root': ['dir1', 'dir2'],
    'dir1': ['file1', 'dir3'],
    'dir2': ['file2'],
    'dir3': ['file3']
}

inicio = 'root'
objetivo = 'file3'

# Llamar a la función y mostrar el resultado
```

# Ejercicio para A\*

**Título**: Ruta óptima en un mapa

**Descripción**: En un mapa, hay varios puntos de interés conectados por caminos con diferentes longitudes. Utiliza el algoritmo A\* para encontrar la ruta más eficiente entre dos puntos, considerando una heurística para guiar la búsqueda.

**Grafo de ejemplo**:

```python
grafo = {
    'A': {'B': 5, 'C': 3},
    'B': {'A': 5, 'D': 2, 'E': 4},
    'C': {'A': 3, 'F': 1},
    'D': {'B': 2, 'E': 1},
    'E': {'B': 4, 'D': 1, 'F': 3},
    'F': {'C': 1, 'E': 3}
}

# Heurística: distancia euclidiana aproximada
heuristica = {
    'A': 10,
    'B': 8,
    'C': 6,
    'D': 5,
    'E': 3,
    'F': 0
}
```

**Tarea**:
1. Implementa el algoritmo A\* en Python para encontrar la ruta más eficiente entre 'A' y 'F'.
2. Explica cómo se utiliza la heurística para guiar la búsqueda.
3. Discute las ventajas de usar A\* sobre Dijkstra en este tipo de problemas.

**Código base**:

```python
import heapq

def a_estrella(grafo, inicio, fin, heuristica):
    # Implementación del algoritmo
    pass

grafo = {
    'A': {'B': 5, 'C': 3},
    'B': {'A': 5, 'D': 2, 'E': 4},
    'C': {'A': 3, 'F': 1},
    'D': {'B': 2, 'E': 1},
    'E': {'B': 4, 'D': 1, 'F': 3},
    'F': {'C': 1, 'E': 3}
}

heuristica = {
    'A': 10,
    'B': 8,
    'C': 6,
    'D': 5,
    'E': 3,
    'F': 0
}

inicio = 'A'
fin = 'F'

# Llamar a la función y mostrar el resultado
```

# Ejercicio para Bellman-Ford

**Título**: Detección de ciclos negativos en una red financiera

**Descripción**: En una red financiera, las transacciones entre entidades pueden tener valores negativos si implican deudas. Utiliza el algoritmo de Bellman-Ford para detectar ciclos negativos en esta red.

**Grafo de ejemplo**:

```python
grafo = {
    'A': {'B': -1, 'C':  4},
    'B': {'C':  3, 'D':  2, 'E':  2},
    'C': {},
    'D': {'B':  1, 'C':  5},
    'E': {'D': -3}
}
```

**Tarea**:
1. Implementa el algoritmo de Bellman-Ford en Python para detectar ciclos negativos en el grafo.
2. Explica cómo se manejan los pesos negativos y cómo se detectan los ciclos.
3. Discute las diferencias entre Bellman-Ford y Dijkstra en este tipo de problemas.

**Código base**:

```python
def bellman_ford(grafo, inicio):
    # Implementación del algoritmo
    pass

grafo = {
    'A': {'B': -1, 'C':  4},
    'B': {'C':  3, 'D':  2, 'E':  2},
    'C': {},
    'D': {'B':  1, 'C':  5},
    'E': {'D': -3}
}

inicio = 'A'

# Llamar a la función y mostrar el resultado
```

# Ejercicio para Floyd-Warshall

**Título**: Matriz de caminos más cortos en una red de comunicaciones

**Descripción**: En una red de comunicaciones, los nodos están conectados con diferentes costos de transmisión. Utiliza el algoritmo de Floyd-Warshall para encontrar la matriz de caminos más cortos entre todos los pares de nodos.

**Grafo de ejemplo**:

```python
grafo = {
    'A': {'B': 5, 'C': float('inf')},
    'B': {'A': 5, 'C': 2, 'D': float('inf')},
    'C': {'A': float('inf'), 'B': 2, 'D': 1},
    'D': {'B': float('inf'), 'C': 1}
}
```

**Tarea**:
1. Implementa el algoritmo de Floyd-Warshall en Python para calcular la matriz de caminos más cortos.
2. Explica cómo se actualizan las distancias entre los nodos.
3. Discute las ventajas de usar Floyd-Warshall sobre Dijkstra para encontrar caminos entre todos los pares de nodos.

**Código base**:

```python
def floyd_warshall(grafo):
    # Implementación del algoritmo
    pass

grafo = {
    'A': {'B': 5, 'C': float('inf')},
    'B': {'A': 5, 'C': 2, 'D': float('inf')},
    'C': {'A': float('inf'), 'B': 2, 'D': 1},
    'D': {'B': float('inf'), 'C': 1}
}

# Llamar a la función y mostrar el resultado
```

---

