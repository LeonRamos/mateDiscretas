# Lógica Proposicional

La **lógica proposicional** es un sistema formal dentro de la lógica matemática que estudia las proposiciones y sus relaciones mediante conectores lógicos. 

## Conceptos Básicos

### Proposición
Una **proposición** es una oración que puede ser verdadera o falsa, pero no ambas al mismo tiempo. Ejemplos:
- "El cielo es azul." (Puede ser verdadera o falsa dependiendo del contexto)
- "2 + 2 = 4." (Siempre verdadera)
- "La Tierra es plana." (Siempre falsa)

### Conectores Lógicos
Los conectores lógicos permiten combinar proposiciones para formar expresiones más complejas.

| Símbolo | Nombre            | Ejemplo                  |
|---------|-----------------|--------------------------|
| ¬       | Negación        | ¬P (No P)               |
| ∧       | Conjunción      | P ∧ Q (P y Q)           |
| ∨       | Disyunción      | P ∨ Q (P o Q)           |
| →       | Implicación     | P → Q (Si P entonces Q) |
| ↔       | Bicondicional   | P ↔ Q (P si y solo si Q) |

## Tablas de Verdad
Las tablas de verdad se utilizan para analizar el valor de verdad de una expresión lógica en función de sus componentes.

Ejemplo de tabla de verdad para la conjunción (P ∧ Q):

| P | Q | P ∧ Q |
|---|---|-------|
| V | V | V     |
| V | F | F     |
| F | V | F     |
| F | F | F     |

## Leyes Fundamentales
Existen varias leyes importantes en la lógica proposicional, como:
- **Ley de la Doble Negación**: ¬(¬P) ↔ P
- **Ley de De Morgan**: 
  - ¬(P ∧ Q) ↔ (¬P ∨ ¬Q)
  - ¬(P ∨ Q) ↔ (¬P ∧ ¬Q)
- **Idempotencia**: 
  - P ∧ P ↔ P
  - P ∨ P ↔ P

## Aplicaciones
La lógica proposicional se utiliza en diversas áreas, como:
- **Circuitos Digitales** (diseño de compuertas lógicas)
- **Inteligencia Artificial** (razonamiento automático)
- **Verificación de Software** (demostraciones formales de programas)
- **Bases de Datos** (consultas lógicas y reglas de inferencia)

## Ejemplo de Uso en Python
Podemos implementar operaciones de lógica proposicional en Python con expresiones booleanas:

```python
P = True
Q = False

# Conjunción (AND)
print(P and Q)  # False

# Disyunción (OR)
print(P or Q)   # True

# Negación (NOT)
print(not P)    # False
```

## Referencias
- Introducción a la Lógica Matemática - Irving M. Copi
- "Discrete Mathematics and Its Applications" - Kenneth H. Rosen
