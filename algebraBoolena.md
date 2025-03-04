

![Awesome](https://img.shields.io/badge/-Awesome-blueviolet) ![Matemáticas](https://img.shields.io/badge/-Matem%C3%A1ticas-orange) ![MATLAB](https://img.shields.io/badge/-MATLAB-blue) ![Circuitos Digitales](https://img.shields.io/badge/-Circuitos%20Digitales-red) ![Álgebra Booleana](https://img.shields.io/badge/-%C3%81lgebra%20Booleana-green)
# 📖 Álgebra Booleana

La [álgebra booleana](https://youtu.be/p58C7OWe3Xk?si=-7xC_UgKonFeLI-M) es una rama del álgebra que se utiliza para representar y manipular expresiones lógicas. Desarrollada por [George Boole en 1847](https://en.wikipedia.org/wiki/George_Boole), esta estructura algebraica esquematiza operaciones lógicas y ha sido fundamental en el desarrollo de la electrónica digital y la programación.

## Características principales

- Utiliza solo dos valores: [verdadero (1) y falso (0)](https://static.platzi.com/media/user_upload/True%20y%20false%20diagrama-84f9825e-0af1-464d-aa9a-771417d12318.jpg).
- Emplea operadores lógicos como [AND (∧), OR (∨) y NOT (¬)](https://saberpunto.com/wp-content/uploads/operadores-logicos-and-or-y-not-en-expresiones-logicas-cl.webp).
- Se basa en variables booleanas que pueden tomar [valores de 1 o 0.](https://www.google.com/url?sa=i&url=https%3A%2F%2Felectronicalugo.com%2Ffunciones-booleanas-usando-puertas-logicas%2F&psig=AOvVaw31HNY8VyMrwT-0mGAEYTwK&ust=1741199970667000&source=images&cd=vfe&opi=89978449&ved=0CBQQjRxqFwoTCICju8mJ8YsDFQAAAAAdAAAAABAX)


## Operaciones básicas

1. Complemento [(NOT)](https://www.geogebra.org/m/f9rv4dpn#material/q8dkbs2p): Negación de una variable.
2. Suma lógica [(OR)](https://ielectel.com/wp-content/uploads/2023/12/diag_OR.png): Disyunción entre variables.
3. Producto lógico [(AND)](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEh7uO6f2M4XkeyJ78nqzG-Ee62Kscc6rfrsaCmH_zm5mC1zKmJOfThXDjCN1iDKmsfEzpp_EPtv1wgQXaqcka46CWk7tvKj_zdyIa-77iRtDfSAGdU4-wJPpTWTxfsX9F4VZNLMz8zF20c/s1600/2.png): Conjunción entre variables.

## Aplicaciones

El álgebra booleana tiene diversas aplicaciones, incluyendo:

- **🔧 Diseño de circuitos digitales:**
Fundamental para crear y optimizar circuitos lógicos en dispositivos electrónicos. Permite simplificar funciones lógicas, reduciendo componentes y mejorando la eficiencia energética.

Ejemplo: En el diseño de un sumador binario de 1 bit, se utiliza la expresión S = A XOR B XOR Cin, donde S es la suma, A y B son los bits a sumar, y Cin es el acarreo de entrada. Esta simplificación permite implementar el circuito con menos compuertas lógicas.

- **💻 Programación y lenguajes informáticos:**
Esencial para controlar el flujo de ejecución y tomar decisiones basadas en condiciones lógicas. Se utiliza en estructuras de control, operaciones de bits y optimización de código.

Ejemplo: En un programa de control de acceso:
```python
if (esUsuarioAutorizado and tieneContraseñaCorrecta) or esAdministrador:
    permitirAcceso()
```

- **🔢 Teoría de conjuntos:**
Proporciona una base matemática para operaciones y relaciones entre conjuntos. Las leyes del álgebra booleana se aplican directamente a operaciones como unión, intersección y complemento.

Ejemplo: En una base de datos de biblioteca, se podría buscar:
(Ficción ∩ Siglo XX) ∪ (No-Ficción ∩ Historia)

- **🧠 Lógica proposicional:**
Permite representar y evaluar proposiciones lógicas complejas. Se utiliza para analizar argumentos lógicos y es fundamental en sistemas de inferencia en inteligencia artificial.

Ejemplo: En un sistema experto médico:
(FiebreAlta ∧ DolorGarganta ∧ TosIntensa) → PosibleGripe

Donde cada proposición representa un síntoma y la flecha indica una implicación lógica hacia un posible diagnóstico.


## 📖 Teoremas y postulados

Los teoremas y postulados son fundamentales para la simplificación de funciones booleanas.

### Postulados

Los [postulados](https://angelmicelti.github.io/4ESO/EDI/33_lgebra_de_boole.html) son enunciados que se toman como punto de partida sin necesidad de demostración. Los principales postulados del álgebra booleana son:

1. Elemento identidad:
    - A + 0 = A (para la suma)
    - A · 1 = A (para el producto)
2. Conmutatividad:
    - A + B = B + A
    - A · B = B · A
3. Asociatividad:
    - (A + B) + C = A + (B + C)
    - (A · B) · C = A · (B · C)
4. Distributividad:
    - A · (B + C) = (A · B) + (A · C)
    - A + (B · C) = (A + B) · (A + C)
5. Complemento:
Para cada valor A existe un valor Ā tal que:
    - A · Ā = 0
    - A + Ā = 1

### Teoremas

Los [teoremas](https://www.uhu.es/rafael.lopezahumada/descargas/tema3_fund_0405.pdf) son proposiciones que se deducen de los postulados. Algunos de los teoremas más importantes del álgebra booleana son:

1. Idempotencia:
    - A + A = A
    - A · A = A
2. Elementos nulos:
    - A + 1 = 1
    - A · 0 = 0
3. Involución:
    - (Ā)' = A
4. Leyes de De Morgan:
    - (A + B)' = A' · B'
    - (A · B)' = A' + B'
5. Absorción:
    - A + (A · B) = A
    - A · (A + B) = A
6. Dualidad:
Cualquier expresión algebraica deducida de los postulados del álgebra booleana sigue siendo válida si se intercambian los operadores suma y producto, así como los elementos 0 y 1.

Claro, aquí tienes tres ejercicios resueltos para cada uno de los temas principales de teoremas y postulados del álgebra booleana. Los resolveré paso a paso para una mejor comprensión.

# 🖍️Ejemplos:
## Postulados del Álgebra Booleana

### Ejercicio 1: Elemento identidad

Demostrar que A + 0 = A

Pasos:
1. Partimos de la expresión A + 0
2. Por el postulado del elemento identidad para la suma, sabemos que cualquier variable sumada con 0 es igual a sí misma
3. Por lo tanto, A + 0 = A

### Ejercicio 2: Conmutatividad

Demostrar que A · B = B · A

Pasos:
1. Partimos de la expresión A · B
2. Por el postulado de conmutatividad para el producto, sabemos que el orden de los factores no altera el producto
3. Por lo tanto, A · B = B · A

### Ejercicio 3: Distributividad

Demostrar que A · (B + C) = (A · B) + (A · C)

Pasos:
1. Partimos de la expresión A · (B + C)
2. Por el postulado de distributividad, sabemos que podemos distribuir A sobre la suma de B y C
3. Esto resulta en (A · B) + (A · C)
4. Por lo tanto, A · (B + C) = (A · B) + (A · C)

## Teoremas del Álgebra Booleana

### Ejercicio 1: Idempotencia

Demostrar que A + A = A

Pasos:
1. Partimos de la expresión A + A
2. Por el teorema de idempotencia, sabemos que cualquier variable sumada consigo misma es igual a sí misma
3. Por lo tanto, A + A = A

### Ejercicio 2: Leyes de De Morgan

Demostrar que (A + B)' = A' · B'

Pasos:
1. Partimos de la expresión (A + B)'
2. Aplicamos la primera ley de De Morgan, que establece que el complemento de una suma es igual al producto de los complementos
3. Esto resulta en A' · B'
4. Por lo tanto, (A + B)' = A' · B'

### Ejercicio 3: Absorción

Demostrar que A + (A · B) = A

Pasos:
1. Partimos de la expresión A + (A · B)
2. Aplicamos el teorema de absorción, que establece que una variable sumada con el producto de sí misma y otra variable es igual a la variable original
3. Por lo tanto, A + (A · B) = A

Estos ejercicios cubren algunos de los postulados y teoremas más importantes del álgebra booleana. Practicar con estos ejemplos ayudará a comprender mejor cómo aplicar estas reglas en problemas más complejos.

> [!NOTE]
> [ 📚 Revisa la plataforma de Classroom y completa los ejercicios propuestos para los temas 'Teoremas y Postulados', asegurándote de entregarlos en tiempo y forma, siguiendo la rúbrica establecida.](https://classroom.google.com/c/NzQ4NzIwNTAxMTY0)
## 📖 Optimización de expresiones booleanas

La optimización de expresiones booleanas busca simplificar funciones lógicas para implementarlas de manera más eficiente.

### Métodos de optimización

1. **Método algebraico**: Utiliza los postulados y teoremas del álgebra de Boole para simplificar las expresiones.
2. **Método gráfico**: Emplea el mapa de Karnaugh, una representación visual de la tabla de verdad que facilita la identificación de términos simplificables.

### Técnicas de simplificación

- **Factorización**: Identificar términos comunes en diferentes partes de la expresión.
- **Absorción**: Aplicar leyes de absorción para eliminar términos redundantes.

# 🖍️Ejemplos:

## Métodos de optimización

### Ejercicio 1: Método algebraico

Simplificar la expresión booleana: F = A'B + AB + A'C

Paso 1: Identificar términos comunes
- A'B y AB tienen B en común
- A'B y A'C tienen A' en común

Paso 2: Factorizar B
F = B(A' + A) + A'C

Paso 3: Aplicar el teorema de complemento (A' + A = 1)
F = B(1) + A'C

Paso 4: Simplificar
F = B + A'C

Resultado final: F = B + A'C

### Ejercicio 2: Método del mapa de Karnaugh

Simplificar la función: F = A'B'C + A'BC + AB'C + ABC

Paso 1: Construir el mapa de Karnaugh
```
   BC
A  00 01 11 10
0  0  1  1  0
1  0  1  1  0
```

Paso 2: Identificar grupos de unos adyacentes
- Se forma un grupo de 4 unos en la columna BC = 01 y BC = 11

Paso 3: Determinar la expresión simplificada
- El grupo identificado elimina la variable A, quedando BC

Resultado final: F = BC

### Ejercicio 3: Método de Quine-McCluskey

Simplificar la función: F = ∑m(0,1,2,5,7,8,10,15)

Paso 1: Listar los minitérminos en binario
0000, 0001, 0010, 0101, 0111, 1000, 1010, 1111

Paso 2: Agrupar por número de unos
0 unos: 0000
1 uno:  0001, 0010, 1000
2 unos: 0101, 1010
3 unos: 0111
4 unos: 1111

Paso 3: Comparar términos adyacentes y crear implicantes primos
0-00, -000, 00-0, 10-0

Paso 4: Crear tabla de implicantes primos
```
    0 1 2 5 7 8 10 15
0-00 X X
-000 X X
00-0 X X
10-0     X   X
```

Paso 5: Seleccionar implicantes primos esenciales
0-00, -000, 10-0

Resultado final: F = A'B'C' + A'B'D' + AB'C'

## Técnicas de simplificación

### Ejercicio 1: Teorema de absorción

Simplificar la expresión: F = A + AB

Paso 1: Identificar el término que puede ser absorbido
- AB puede ser absorbido por A

Paso 2: Aplicar el teorema de absorción (A + AB = A)
F = A

Resultado final: F = A

### Ejercicio 2: Leyes de De Morgan

Simplificar la expresión: F = (A + B)'(C + D)'

Paso 1: Aplicar la primera ley de De Morgan a (A + B)'
F = (A'B')(C + D)'

Paso 2: Aplicar la primera ley de De Morgan a (C + D)'
F = (A'B')(C'D')

Paso 3: Aplicar la ley distributiva
F = A'B'C'D'

Resultado final: F = A'B'C'D'

### Ejercicio 3: Complemento y doble negación

Simplificar la expresión: F = A + (A' + B)'

Paso 1: Aplicar la ley de De Morgan a (A' + B)'
F = A + (AB')'

Paso 2: Aplicar la ley de doble negación
F = A + AB

Paso 3: Aplicar el teorema de absorción (A + AB = A)
F = A

Resultado final: F = A
> [!NOTE]
> [ 📚 Revisa la plataforma de Classroom y completa los ejercicios propuestos para el tema 'Optimización de Expresiones Booleanas', asegurándote de entregarlos en tiempo y forma, siguiendo la rúbrica establecida.](https://classroom.google.com/c/NzQ4NzIwNTAxMTY0)

## 📖 Minitérminos y maxitérminos

Los [minitérminos y maxitérminos](https://nlaredo.tecnm.mx/takeyas/Apuntes/Matematicas_Discretas/Apuntes/Algebra_Booleana.pdf) son formas canónicas de representar funciones booleanas:

### Minitérminos

- Son productos de variables donde cada variable aparece una sola vez, ya sea en forma directa o negada.
- Representan combinaciones específicas de entradas que hacen que la función sea verdadera.
- Se denotan como m₀, m₁, m₂, etc.


### Maxitérminos

- Son sumas de variables donde cada variable aparece una sola vez, ya sea en forma directa o negada.
- Representan combinaciones específicas de entradas que hacen que la función sea falsa.
- Se denotan como M₀, M₁, M₂, etc.

# 🖍️Ejemplos:
## Métodos de optimización

### Ejercicio 1: Método algebraico

Simplificar la expresión booleana: F = A'B + AB + A'C

Paso 1: Identificar términos comunes
- A'B y AB tienen B en común
- A'B y A'C tienen A' en común

Paso 2: Factorizar B
F = B(A' + A) + A'C

Paso 3: Aplicar el teorema de complemento (A' + A = 1)
F = B(1) + A'C

Paso 4: Simplificar
F = B + A'C

Resultado final: F = B + A'C

### Ejercicio 2: Método del mapa de Karnaugh

Simplificar la función: F = A'B'C + A'BC + AB'C + ABC

Paso 1: Construir el mapa de Karnaugh
```
   BC
A  00 01 11 10
0  0  1  1  0
1  0  1  1  0
```

Paso 2: Identificar grupos de unos adyacentes
- Se forma un grupo de 4 unos en la columna BC = 01 y BC = 11

Paso 3: Determinar la expresión simplificada
- El grupo identificado elimina la variable A, quedando BC

Resultado final: F = BC

### Ejercicio 3: Método de Quine-McCluskey

Simplificar la función: F = ∑m(0,1,2,5,7,8,10,15)

Paso 1: Listar los minitérminos en binario
0000, 0001, 0010, 0101, 0111, 1000, 1010, 1111

Paso 2: Agrupar por número de unos
0 unos: 0000
1 uno:  0001, 0010, 1000
2 unos: 0101, 1010
3 unos: 0111
4 unos: 1111

Paso 3: Comparar términos adyacentes y crear implicantes primos
0-00, -000, 00-0, 10-0

Paso 4: Crear tabla de implicantes primos
```
    0 1 2 5 7 8 10 15
0-00 X X
-000 X X
00-0 X X
10-0     X   X
```

Paso 5: Seleccionar implicantes primos esenciales
0-00, -000, 10-0

Resultado final: F = A'B'C' + A'B'D' + AB'C'

## Técnicas de simplificación

### Ejercicio 1: Teorema de absorción

Simplificar la expresión: F = A + AB

Paso 1: Identificar el término que puede ser absorbido
- AB puede ser absorbido por A

Paso 2: Aplicar el teorema de absorción (A + AB = A)
F = A

Resultado final: F = A

### Ejercicio 2: Leyes de De Morgan

Simplificar la expresión: F = (A + B)'(C + D)'

Paso 1: Aplicar la primera ley de De Morgan a (A + B)'
F = (A'B')(C + D)'

Paso 2: Aplicar la primera ley de De Morgan a (C + D)'
F = (A'B')(C'D')

Paso 3: Aplicar la ley distributiva
F = A'B'C'D'

Resultado final: F = A'B'C'D'

### Ejercicio 3: Complemento y doble negación

Simplificar la expresión: F = A + (A' + B)'

Paso 1: Aplicar la ley de De Morgan a (A' + B)'
F = A + (AB')'

Paso 2: Aplicar la ley de doble negación
F = A + AB

Paso 3: Aplicar el teorema de absorción (A + AB = A)
F = A

Resultado final: F = A

> [!NOTE]
> [ 📚 Revisa la plataforma de Classroom y completa los ejercicios propuestos para los temas 'Minitérminos y maxitérminos', asegurándote de entregarlos en tiempo y forma, siguiendo la rúbrica establecida.](https://classroom.google.com/c/NzQ4NzIwNTAxMTY0)

## 📖 Representación de expresiones booleanas con circuitos lógicos

La representación de expresiones booleanas con circuitos lógicos implica traducir una expresión booleana en un circuito físico utilizando compuertas lógicas.

### Proceso de representación

1. Análisis de la expresión booleana: Identificar las variables de entrada y los operadores lógicos utilizados.
2. Selección de compuertas lógicas: Compuertas básicas (OR, AND, NOT) y derivadas (NOR, NAND).
3. Implementación del circuito: Conectar las entradas a las compuertas correspondientes y conectar la salida final.

### Tipos de compuertas lógicas

- Compuerta OR: Salida Y = A + B
- Compuerta AND: Salida Y = A · B
- Compuerta NOT: Salida Y = A'

### 🧮 Tablas de Verdad de Compuertas Lógicas

| A | B | OR (A + B) | AND (A · B) | NOT (¬A) | NOR (¬(A + B)) | NAND (¬(A · B)) |
|---|---|------------|------------|---------|---------------|---------------|
| 0 | 0 |     0      |     0      |    1    |       1       |       1       |
| 0 | 1 |     1      |     0      |    1    |       0       |       1       |
| 1 | 0 |     1      |     0      |    0    |       0       |       1       |
| 1 | 1 |     1      |     1      |    0    |       0       |       0       |

#### ✍️ Expresiones Booleanas
- **🔹 OR:** \( A + B \)
- **🔹 AND:** \( A \cdot B \)
- **🔹 NOT:** \( \neg A \) (solo requiere una entrada)
- **🔹 NOR:** \( \neg (A + B) \)
- **🔹 NAND:** \( \neg (A \cdot B) \)


## 🖍️ Ejemplo de implementación

Para la expresión booleana "X · Y + Z'":

1. Usar una compuerta AND para X · Y
2. Usar una compuerta NOT para Z'
3. Conectar las salidas de estas compuertas a una compuerta OR

### Formas canónicas

Las expresiones booleanas pueden representarse en formas canónicas para facilitar su implementación en circuitos:

1. Suma de productos (SOP): Utiliza minitérminos
2. Producto de sumas (POS): Utiliza maxitérminos

### Optimización de circuitos

La optimización de circuitos lógicos busca reducir la complejidad y mejorar el rendimiento:

1. Simplificación algebraica: Aplicar leyes y teoremas del álgebra booleana.
2. Mapas de Karnaugh: Método gráfico para simplificar funciones lógicas.
3. Uso de compuertas universales: NAND o NOR para implementar cualquier función lógica.

La representación eficiente de expresiones booleanas en circuitos lógicos es crucial para el diseño de sistemas digitales eficientes y compactos.

> [!NOTE]
> [ 📚 Revisa la plataforma de Classroom y completa los ejercicios propuestos para el tema 'Optimización de circuitoss', asegurándote de entregarlos en tiempo y forma, siguiendo la rúbrica establecida.](https://classroom.google.com/c/NzQ4NzIwNTAxMTY0)
