# 📊 Representación de los Grafos

![Matemáticas](https://img.shields.io/badge/Matemáticas-Teoría%20de%20Grafos-blue) ![Computación](https://img.shields.io/badge/Computación-Implementación%20en%20Python-green)

## 📖 Introducción
La **representación de grafos** es fundamental tanto en matemáticas como en computación. En este capítulo se exploran ambas perspectivas, proporcionando ejemplos prácticos para cada una.

## 📐 Representación Matemática
Los grafos se pueden representar mediante:

### 🔹 Matriz de Adyacencia
Una matriz de adyacencia indica con **1** si hay una arista entre dos vértices y con **0** si no existe conexión. Para grafos no dirigidos, la matriz es simétrica.

**Ejemplo:**
```
    A B C
A [ 0 1 1 ]
B [ 1 0 1 ]
C [ 1 1 0 ]
```

### 🔹 Matriz de Incidencia
Cada fila representa un vértice y cada columna una arista. Se indica con **1** si el vértice está conectado por la arista.

**Ejemplo:**
```
    e1 e2 e3
A [ 1 1 0 ]
B [ 1 0 1 ]
C [ 0 1 1 ]
```

### 🔹 Lista de Adyacencia
Una lista de adyacencia asocia cada vértice con una lista de sus vértices adyacentes.

**Ejemplo:**
```
A: [B, C]
B: [A, C]
C: [A, B]
```

## 💻 Representación Computacional
En computación, estas representaciones se implementan mediante estructuras de datos eficientes.

### 🐍 Implementación en Python
```python
import numpy as np

# Matriz de Adyacencia
matriz_adyacencia = np.array([
    [0, 1, 1],
    [1, 0, 1],
    [1, 1, 0]
])
print(matriz_adyacencia)

# Matriz de Incidencia
matriz_incidencia = np.array([
    [1, 1, 0],
    [1, 0, 1],
    [0, 1, 1]
])
print(matriz_incidencia)

# Lista de Adyacencia
lista_adyacencia = {
    'A': ['B', 'C'],
    'B': ['A', 'C'],
    'C': ['A', 'B']
}
for v, adj in lista_adyacencia.items():
    print(f"{v}: {adj}")
```

## 🔎 Conclusión
La representación de grafos es crucial tanto en el ámbito teórico como en el computacional. Elegir la representación adecuada facilita el análisis y la implementación de algoritmos eficientes para resolver problemas complejos. 🚀
