Los árboles con peso se refieren a estructuras donde cada nodo tiene un valor asociado (peso) y el peso total del árbol es la suma de estos valores. Sin embargo, en el contexto de estructuras de datos, el "peso" también puede referirse al número total de nodos en el árbol. Implementaremos ambas interpretaciones.

## Implementación de un árbol con peso en Python
Crearemos un árbol binario con métodos para calcular su peso (cantidad de nodos) y realizar recorridos:

```python
class Nodo:
    def __init__(self, valor):
        self.valor = valor
        self.izquierda = None
        self.derecha = None

class ArbolPeso:
    def __init__(self):
        self.raiz = None

    def insertar(self, valor):
        if self.raiz is None:
            self.raiz = Nodo(valor)
        else:
            self._insertar_recursivo(self.raiz, valor)

    def _insertar_recursivo(self, nodo, valor):
        if valor < nodo.valor:
            if nodo.izquierda is None:
                nodo.izquierda = Nodo(valor)
            else:
                self._insertar_recursivo(nodo.izquierda, valor)
        else:
            if nodo.derecha is None:
                nodo.derecha = Nodo(valor)
            else:
                self._insertar_recursivo(nodo.derecha, valor)

    def peso(self, nodo):
        if nodo is None:
            return 0
        return 1 + self.peso(nodo.izquierda) + self.peso(nodo.derecha)

    def preorden(self, nodo):
        if nodo:
            print(nodo.valor, end=" ")
            self.preorden(nodo.izquierda)
            self.preorden(nodo.derecha)

    def inorden(self, nodo):
        if nodo:
            self.inorden(nodo.izquierda)
            print(nodo.valor, end=" ")
            self.inorden(nodo.derecha)

    def postorden(self, nodo):
        if nodo:
            self.postorden(nodo.izquierda)
            self.postorden(nodo.derecha)
            print(nodo.valor, end=" ")

# Ejemplo de uso
arbol = ArbolPeso()
numeros = [15, 10, 20, 8, 12, 17, 25]
for n in numeros:
    arbol.insertar(n)

print("Recorridos:")
print("Preorden:", end=" ")
arbol.preorden(arbol.raiz)
print("\nInorden:", end=" ")
arbol.inorden(arbol.raiz)
print("\nPostorden:", end=" ")
arbol.postorden(arbol.raiz)
print("\nPeso total del árbol:", arbol.peso(arbol.raiz))
```

## Explicación paso a paso
1. **Estructura del Nodo**:
   - Cada nodo almacena un valor y tiene referencias a sus hijos izquierdo y derecho
   - Constructor inicializa con `valor` y hijos `None`

2. **Inserción de valores**:
   - Método `insertar` maneja la raíz
   - `_insertar_recursivo` ordena valores menores a la izquierda y mayores/iguales a la derecha

3. **Cálculo de peso**:
   - Función recursiva que suma 1 (nodo actual) + peso subárbol izquierdo + peso subárbol derecho
   - Caso base: nodo `None` retorna 0

4. **Recorridos**:
   - **Preorden**: Raíz → Subárbol izquierdo → Subárbol derecho
   - **Inorden**: Subárbol izquierdo → Raíz → Subárbol derecho
   - **Postorden**: Subárbol izquierdo → Subárbol derecho → Raíz

## Resultado esperado en Google Colab
```
Recorridos:
Preorden: 15 10 8 12 20 17 25 
Inorden: 8 10 12 15 17 20 25 
Postorden: 8 12 10 17 25 20 15 
Peso total del árbol: 7
```

## Caso de ejemplo
Para el árbol creado con valores [15, 10, 20, 8, 12,6]:
- **Preorden** comienza en la raíz (15), luego izquierda completa antes de derecha
- **Inorden** muestra valores ordenados
- **Postorden** procesa hijos antes que raíces
- **Peso** cuenta 7 nodos (1 raíz + 3 izquierdos + 3 derechos)

