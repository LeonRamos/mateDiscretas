

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![AI](https://img.shields.io/badge/AI-Deep%20Learning-blue?style=for-the-badge)
![Scrum](https://img.shields.io/badge/Scrum-Agile-blue?style=for-the-badge)


## Introducción a los Árboles

Un **árbol** es una estructura de datos no lineal que consiste en nodos conectados por aristas, donde:

1. Existe un nodo especial llamado **raíz**, que es el punto de partida del árbol.
2. Cada nodo (excepto la raíz) tiene exactamente un padre.
3. No hay ciclos (es decir, no se puede volver al mismo nodo por las aristas).

Un árbol es útil en muchas aplicaciones, como representar jerarquías, rutas, o estructuras de datos como tablas de decisión.

---

## Componentes y Propiedades de los Árboles

### Componentes principales:
1. **Raíz**: El nodo principal desde donde se inicia el árbol.
2. **Hijos**: Los nodos directamente conectados a un nodo superior (padre).
3. **Padre**: El nodo inmediatamente superior a un nodo hijo.
4. **Hojas**: Nodos sin hijos.
5. **Nivel**: La profundidad de un nodo desde la raíz.
6. **Altura**: La distancia máxima desde la raíz hasta cualquier hoja.
7. **Subárbol**: Cualquier nodo y sus descendientes forman un subárbol.

### Propiedades importantes:
1. Si un árbol tiene \( n \) nodos, tendrá exactamente \( n-1 \) aristas.
2. La altura de un árbol con una única hoja es 0.
3. Un árbol binario perfecto tiene todos sus niveles completamente llenos.

---

## Clasificación de los Árboles

### Clasificación por Altura

1. **Árbol de altura \( h \):**
   - La altura de un árbol es la longitud del camino más largo desde la raíz hasta una hoja.
   - Ejemplo: Si un árbol tiene la raíz en el nivel 0 y hojas en el nivel 3, la altura del árbol es 3.

2. **Árbol equilibrado:**
   - La diferencia entre las alturas de los subárboles izquierdo y derecho de cualquier nodo es como máximo 1.

### Clasificación por Número de Nodos

1. **Árbol binario completo:**
   - Cada nodo tiene exactamente 0 o 2 hijos.

2. **Árbol binario perfecto:**
   - Todos los niveles están llenos completamente.

3. **Árbol binario degenerado:**
   - Cada nodo tiene un único hijo, formando una estructura lineal similar a una lista enlazada.

---

## Ejemplos Explicados

### Ejemplo 1: Crear un Árbol Binario Completo

Dado el conjunto de datos \( \{A, B, C, D, E, F, G\} \), construyamos un árbol binario completo:

1. Elige \( A \) como la raíz.
2. Añade \( B \) y \( C \) como hijos de \( A \).
3. Añade \( D \) y \( E \) como hijos de \( B \).
4. Añade \( F \) y \( G \) como hijos de \( C \).

**Árbol resultante:**
```
        A
       / \
      B   C
     / \ / \
    D  E F  G
```

- **Altura**: 2 (desde la raíz \( A \) hasta cualquier hoja).
- **Número de nodos**: 7.

### Ejemplo 2: Verificar si un Árbol es Equilibrado

Dado el árbol:
```
        X
       / \
      Y   Z
         / \
        P   Q
```
1. Calcula la altura del subárbol izquierdo (\( Y \)):
   - \( Y \) es una hoja, por lo que su altura es 0.

2. Calcula la altura del subárbol derecho (\( Z \)):
   - La altura de \( P \) y \( Q \) es 0.
   - La altura de \( Z \) es 1 (mayor altura entre sus hijos más 1).

3. La diferencia de alturas es \( |1 - 0| = 1 \), por lo que el árbol es equilibrado.

### Ejemplo 3: Árbol Degenerado

Un árbol donde cada nodo tiene un único hijo:
```
    A
     \
      B
       \
        C
         \
          D
```
- **Altura**: 3.
- **Número de nodos**: 4.

---

## Aplicaciones
1. **Árboles de decisión:** Usados en aprendizaje automático.
2. **Sistemas de archivos:** Representan carpetas y archivos.
3. **Jerarquías:** Organigramas o estructuras jerárquicas.


# Ejercicios Árboles Binarios

---

## Problema 1: Construcción de un Árbol Binario
Dado el siguiente conjunto de datos: \( \{10, 20, 30, 40, 50, 60, 70\} \), construye un árbol binario completo.

### Preguntas:
1. Dibuja el árbol resultante.
2. ¿Cuál es la altura del árbol?
3. ¿Cuántos nodos terminales (hojas) tiene el árbol?

### Solución Esperada:
Un árbol binario completo con altura 2 y 4 nodos terminales.

---

## Problema 2: Recorridos en un Árbol Binario
Dado el siguiente árbol binario:
```
        A
       / \
      B   C
     / \ / \
    D  E F  G
```

### Preguntas:
1. Realiza el recorrido en **preorden** (NLR).
2. Realiza el recorrido en **inorden** (LNR).
3. Realiza el recorrido en **postorden** (LRN).

### Solución Esperada:
- Preorden: \( A, B, D, E, C, F, G \)
- Inorden: \( D, B, E, A, F, C, G \)
- Postorden: \( D, E, B, F, G, C, A \)

---

## Problema 3: Árbol Binario de Búsqueda
Inserta los siguientes números en un árbol binario de búsqueda vacío: \( \{50, 30, 70, 20, 40, 60, 80\} \).

### Preguntas:
1. Dibuja el árbol binario de búsqueda resultante.
2. ¿Cuál es el recorrido **inorden** del árbol?

### Solución Esperada:
Un árbol binario de búsqueda correctamente construido. El recorrido **inorden** debería ser: \( 20, 30, 40, 50, 60, 70, 80 \).

---

## Problema 4: Representación Secuencial
Dado el siguiente árbol binario:
```
        15
       /  \
      10   20
     / \   / \
    8  12 17  25
```

### Preguntas:
1. Representa el árbol en un arreglo secuencial (usando índices para los hijos izquierdo y derecho).
2. Determina la posición en el arreglo para el nodo con valor \( 17 \).

### Solución Esperada:
El árbol debe representarse como un arreglo donde:
- Nodo en índice \( i \): hijo izquierdo en \( 2i \) y hijo derecho en \( 2i + 1 \).
- \( 17 \) está en la posición 6 del arreglo.

---

## Problema 5: Construcción a partir de Recorridos
Los recorridos en preorden e inorden de un árbol binario son:
- **Preorden**: \( G, B, Q, A, C, P, D, E, R \)
- **Inorden**: \( Q, B, C, A, G, P, E, D, R \)

### Preguntas:
1. Construye el árbol binario correspondiente.
2. ¿Cuál es la altura del árbol?
3. Identifica las hojas del árbol.

### Solución Esperada:
Un árbol binario correctamente construido con altura 4 y hojas identificadas.



---

## Referencias
- Rosen, K. H. (2019). *Discrete Mathematics and Its Applications.* McGraw-Hill Education.
- Lipschutz, S. (1998). *Matemáticas Discretas - 3ª edición.* McGraw-Hill Education.
