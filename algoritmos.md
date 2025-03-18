
# Algoritmos de Recorrido y Búsqueda en Grafos 🚀

Te explico paso a paso los algoritmos de recorrido y búsqueda más comunes: el camino más corto (Dijkstra), a lo ancho (BFS) y en profundidad (DFS). Además, incluyo ejemplos en Python para cada uno y una tabla con los principales algoritmos.

---

### 5.3.1 El camino más corto: Dijkstra

**Descripción**:  
Dijkstra es un algoritmo utilizado para encontrar el camino más corto entre dos nodos en un grafo ponderado. Funciona asignando una distancia inicial infinita a todos los nodos excepto al de partida, que es 0. Luego, se actualizan las distancias de los nodos vecinos si se encuentra un camino más corto.

**Ejemplo en Python**:

```python
import heapq

def dijkstra(graph, start):
    distances = {node: float('inf') for node in graph}
    distances[start] = 0
    queue = [(0, start)]
    
    while queue:
        current_distance, current_node = heapq.heappop(queue)
        
        if current_distance > distances[current_node]:
            continue
        
        for neighbor, weight in graph[current_node].items():
            distance = current_distance + weight
            
            if distance < distances[neighbor]:
                distances[neighbor] = distance
                heapq.heappush(queue, (distance, neighbor))
    
    return distances

# Ejemplo de grafo
graph = {
    'A': {'B': 1, 'C': 4},
    'B': {'A': 1, 'C': 2, 'D': 5},
    'C': {'A': 4, 'B': 2, 'D': 1},
    'D': {'B': 5, 'C': 1}
}

print(dijkstra(graph, 'A'))
```

---

### 5.3.2 A lo ancho: BFS

**Descripción**:  
BFS (Breadth-First Search) es un algoritmo que explora todos los nodos a una distancia determinada antes de avanzar a la siguiente capa. Utiliza una cola para gestionar los nodos por visitar.

**Ejemplo en Python**:

```python
from collections import deque

def bfs(graph, start):
    visited = set()
    queue = deque([start])
    visited.add(start)
    
    while queue:
        node = queue.popleft()
        print(node, end=" ")
        
        for neighbor in graph[node]:
            if neighbor not in visited:
                visited.add(neighbor)
                queue.append(neighbor)

# Ejemplo de grafo
graph = {
    'A': ['B', 'C'],
    'B': ['A', 'D', 'E'],
    'C': ['A', 'F'],
    'D': ['B'],
    'E': ['B', 'F'],
    'F': ['C', 'E']
}

bfs(graph, 'A')
```

---

### 5.3.3 En profundidad: DFS

**Descripción**:  
DFS (Depth-First Search) explora un grafo o árbol profundizando lo máximo posible en cada rama antes de retroceder. Puede implementarse de forma recursiva o iterativa.

**Ejemplo en Python (recursivo)**:

```python
def dfs(graph, node, visited=None):
    if visited is None:
        visited = set()
    
    visited.add(node)
    print(node, end=" ")
    
    for neighbor in graph[node]:
        if neighbor not in visited:
            dfs(graph, neighbor, visited)

# Ejemplo de grafo
graph = {
    'A': ['B', 'C'],
    'B': ['A', 'D', 'E'],
    'C': ['A', 'F'],
    'D': ['B'],
    'E': ['B', 'F'],
    'F': ['C', 'E']
}

dfs(graph, 'A')
```

---

### Tabla de algoritmos

| Algoritmo         | Autor                                         | Descripción                                                                                          |
|-------------------|-----------------------------------------------|------------------------------------------------------------------------------------------------------|
| **Dijkstra**      | Edsger W. Dijkstra                            | Encuentra el camino más corto entre dos nodos en un grafo ponderado.                                 |
| **BFS**           | No atribuido específicamente                  | Explora todos los nodos a una distancia determinada antes de avanzar.                               |
| **DFS**           | No atribuido específicamente                  | Explora profundizando lo máximo posible en cada rama antes de retroceder.                             |
| **A\***           | Peter Hart, Nils Nilsson y Bertram Raphael     | Combina Dijkstra con una heurística para encontrar el camino más corto.                              |
| **Bellman-Ford**  | Richard Bellman y Lester Ford                  | Similar a Dijkstra, pero maneja pesos negativos y detecta ciclos negativos.                         |
| **Floyd-Warshall**| Robert Floyd y Stephen Warshall                | Encuentra los caminos más cortos entre todos los pares de nodos en un grafo.                          |

---

Estos algoritmos son fundamentales en la teoría de grafos y tienen aplicaciones en diversas áreas como la logística, las redes sociales y la informática. 😊
```

---
