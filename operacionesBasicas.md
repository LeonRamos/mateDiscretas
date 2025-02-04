# Operaciones Básicas en Sistemas Numéricos

## Operaciones en Sistema Binario

### Suma Binaria

La suma binaria se realiza de manera similar a la suma decimal, pero considerando que solo existen dos dígitos: 0 y 1.

Reglas:
- 0 + 0 = 0
- 0 + 1 = 1
- 1 + 0 = 1
- 1 + 1 = 0 (con acarreo de 1)

Ejemplo: 1011 + 1101

```
  1011
+ 1101
------
 11000
```

Pasos:
1. Sumamos de derecha a izquierda: 1 + 1 = 0 (con acarreo de 1)
2. 1 + 0 + 1 (acarreo) = 0 (con acarreo de 1)
3. 0 + 1 + 1 (acarreo) = 0 (con acarreo de 1)
4. 1 + 1 + 1 (acarreo) = 1 (con acarreo de 1)
5. El último acarreo se coloca a la izquierda: 1

### Resta Binaria

La resta binaria se realiza de manera similar a la resta decimal, pero considerando que solo existen dos dígitos: 0 y 1.

Reglas:
- 0 - 0 = 0
- 1 - 0 = 1
- 1 - 1 = 0
- 0 - 1 = 1 (con préstamo de 1)

Ejemplo: 1011 - 0101

```
  1011
- 0101
------
  0110
```

Pasos:
1. 1 - 1 = 0
2. 1 - 0 = 1
3. 0 - 1 = 1 (con préstamo de 1)
4. 0 (después del préstamo) - 0 = 0

### Multiplicación Binaria

La multiplicación binaria sigue los mismos principios que la decimal, pero con solo dos dígitos.

Reglas:
- 0 × 0 = 0
- 0 × 1 = 0
- 1 × 0 = 0
- 1 × 1 = 1

Ejemplo: 101 × 11

```
    101
  × 11
  -----
    101
   101
  -----
   1111
```

Pasos:
1. Multiplicamos 101 por 1 (último dígito del multiplicador)
2. Multiplicamos 101 por 1 (primer dígito del multiplicador) y desplazamos una posición a la izquierda
3. Sumamos los resultados parciales

### División Binaria

La división binaria se realiza de manera similar a la división larga decimal.

Ejemplo: 1100 ÷ 11

```
    100
11 | 1100
     11
    ---
      00
```

Pasos:
1. Dividimos 110 entre 11: cabe 1 vez
2. Multiplicamos 11 × 1 = 11 y restamos de 110
3. Bajamos el siguiente dígito (0)
4. 00 es menor que 11, por lo que el cociente es 100 y el residuo es 0

## Operaciones en Sistema Octal

Las operaciones en sistema octal son similares a las decimales, pero utilizando dígitos del 0 al 7.

### Suma Octal

Ejemplo: 567 + 243

```
  567
+ 243
-----
 1032
```

Pasos:
1. 7 + 3 = 12, escribimos 2 y llevamos 1
2. 6 + 4 + 1 (acarreo) = 13, escribimos 3 y llevamos 1
3. 5 + 2 + 1 (acarreo) = 10, escribimos 0 y llevamos 1
4. Colocamos el último acarreo: 1

### Resta Octal

Ejemplo: 756 - 243

```
  756
- 243
-----
  513
```

Pasos:
1. 6 - 3 = 3
2. 5 - 4 = 1
3. 7 - 2 = 5

## Operaciones en Sistema Hexadecimal

Las operaciones en sistema hexadecimal utilizan dígitos del 0 al 9 y letras de A a F.

### Suma Hexadecimal

Ejemplo: 3A7 + 58F

```
  3A7
+ 58F
-----
  936
```

Pasos:
1. 7 + F = 16 + 7 = 23, escribimos 6 y llevamos 1
2. A + 8 + 1 (acarreo) = 10 + 8 + 1 = 19, escribimos 3 y llevamos 1
3. 3 + 5 + 1 (acarreo) = 9

### Multiplicación Hexadecimal

Ejemplo: 2A × 3

```
   2A
 × 3
-----
   7E
```

Pasos:
1. 3 × A = 30, escribimos E y llevamos 3
2. 3 × 2 + 3 (acarreo) = 9, escribimos 7


## Para complementar la información sobre operaciones básicas en sistemas numéricos binario, octal y hexadecimal, aquí hay algunos enlaces a videos útiles que ayudan a entender los procedimientos:

### Suma Binaria
- [Suma en sistemas: Decimal, Binario, Octal y Hexadecimal](https://www.youtube.com/watch?v=p9wZXDTf_2M)
- [Aritmética binaria: suma, resta, multiplicación y división](https://www.youtube.com/watch?v=gAieLk1BjDY)

### Resta Binaria
- [Sistemas numéricos. Resta de binarios, octales y hexadecimales](https://www.youtube.com/watch?v=iFCQOLwKZjo)

### Multiplicación y División Binaria
- [Suma, resta, producto y división en binario](https://www.youtube.com/watch?v=uLulA91jt_A)


### Suma y Resta Octal
- [Suma octal - Método #1 - Ejercicio #1](https://www.youtube.com/watch?v=j_Ja5e2IK2c)
- [Suma, resta, producto y división en base octal](https://www.youtube.com/watch?v=y-QzyNKs2Xs)

### Multiplicación y División Octal
- [División Octal, Suma, Resta, Producto y División en Hexadecimal](https://www.youtube.com/watch?v=FWOBMyk5s9c)

### Suma y Resta Hexadecimal
- [Suma, resta, producto y división en hexadecimal](https://www.youtube.com/watch?v=1xeJjcwT9pM)

### Multiplicación y División Hexadecimal
- [División Octal, Suma, Resta, Producto y División en Hexadecimal](https://www.youtube.com/watch?v=FWOBMyk5s9c)

## Conversiones entre Sistemas

- [Conversiones entre sistemas de numeración (Binario, octal y hexadecimal)](https://www.youtube.com/watch?v=o79EZsX6VjU)
- [Cambio de bases entre Decimal, binario, octal y hexadecimal](https://www.youtube.com/watch?v=PyIYn8K9zZQ)
- [Conversión de números entre Sistemas Numéricos - Técnica rápida](https://www.youtube.com/watch?v=QrULhy0P_uU)

### Actividad

1. Abrir un nuevo notebook en Google Colab.

2. Copiar y pegar el siguiente código en una celda:

```python
def to_decimal(number, base):
    return int(str(number), base)

def from_decimal(number, base):
    if base == 2:
        return bin(number)[2:]
    elif base == 8:
        return oct(number)[2:]
    elif base == 16:
        return hex(number)[2:]
    else:
        return str(number)

def calculate(num1, num2, operation, base):
    n1 = to_decimal(num1, base)
    n2 = to_decimal(num2, base)
   
    if operation == '+':
        result = n1 + n2
    elif operation == '-':
        result = n1 - n2
    elif operation == '*':
        result = n1 * n2
    elif operation == '/':
        if n2 == 0:
            return "Error: División por cero"
        result = n1 // n2
    else:
        return "Operación no válida"
   
    return from_decimal(result, base)

bases = {2: "Binario", 8: "Octal", 10: "Decimal", 16: "Hexadecimal"}

while True:
    print("\nCalculadora de Sistemas Numéricos")
    for key, value in bases.items():
        print(f"{key}: {value}")
   
    base = int(input("Seleccione la base numérica: "))
    if base not in bases:
        print("Base no válida")
        continue
   
    num1 = input(f"Ingrese el primer número en base {base}: ")
    num2 = input(f"Ingrese el segundo número en base {base}: ")
    operation = input("Ingrese la operación (+, -, *, /): ")
   
    result = calculate(num1, num2, operation, base)
    print(f"Resultado: {result}")
   
    if input("¿Desea realizar otra operación? (s/n): ").lower() != 's':
        break

print("¡Gracias por usar la calculadora!")
```
