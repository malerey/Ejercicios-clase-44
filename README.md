# 🔄 Estructuras de datos: Matrices

## Ejercicios

### 1 

Crear una función `obtenerNumeroMayorArray` que tome como argumento un array de números y devuelva el mayor número de dicho array.

```javascript
obtenerNumeroMayor([2, 7, 12, 1]) // 12
```

### 2

Crear una función `sumarArray` que tome como argumento un array de números y devuelva la suma de todos los número de dicho array.

```javascript
sumar([4, 5, 10]) // 19
```

### 3 `obtenerNumeroMayor(matriz)`

Crear una función `obtenerNumeroMayor` que tome como argumento un array 2d de números `matriz` y devuelva el mayor número de dicha matriz.

```javascript
obtenerNumeroMayor([
  [2, 7, 12, 1],
  [8, 23],
  [9, 45, 7],
  [22, 3, 24, 4],
]) // 45
```

### 4 `sumar(matriz)`

Crear una función `sumar` que tome como argumento un array 2d de números `matriz` y devuelva la suma de todos los número de dicha matriz.

```javascript
sumar([
  [4, 5],
  [2, 7, 1],
  [8, 10],
]) // 37
```

### 5 `esMatrizCuadrada(matriz)`

Crear una función `esMatrizCuadrada` que tome como argumento un array 2d `matriz` y devuelva `true` si es una matriz cuadrada, es decir, si tiene igual cantidad de filas que de columnas, o `false` si no lo es.

```javascript
esMatrizCuadrada([
  [4, 5],
  [2, 7, 1],
  [8, 10],
]) // false

esMatrizCuadrada([
  [4, 5, 9],
  [2, 7, 1],
  [8, 10, 5],
]) // true
```

### 6 `generarGrillaCuadrada(tamanio)`

Crear una función `generarGrillaCuadrada` que tome como argumentos un número entero y devuelva una matriz de `filas` y `columnas` con la longitud `tamanio`, donde cada ítem de la matriz es un string cualquiera (por ejemplo "hola"). 

```javascript
generarGrillaCuadrada(3) /* 
  [
    ["hola", "hola", hola"], 
    ["hola", "hola", hola"],
    ["hola", "hola", hola"]
  ]
*/
```

### 7 `generarGrillaSimple(filas, columnas)`

Crear una función `generarGrillaSimple` que tome como argumentos un número entero `filas`, un número entero `columnas`, y devuelva una matriz de `filas` filas y `columnas` columnas, donde cada ítem de la matriz es un string cualquiera (por ejemplo, "hola"). 

```javascript
generarGrillaSimple(2, 3) /* 
  [
    ["hola", "hola", hola"],
    ["hola", "hola", hola"],
  ]
*/
```

```javascript
generarGrillaSimple(3, 2) /* 
  [
    ["hola", "hola"],
    ["hola", "hola"],
    ["hola", "hola"],
  ]
*/
```

### 7 `generarGrilla(filas, columnas, items)`

Crear una función `generarGrilla` que tome como argumentos un número entero `filas`, un número entero `columnas` y un array de valores `items`, y devuelva una matriz de `filas` filas y `columnas` columnas, donde cada ítem de la matriz es un ítem _aleatorio_ de `items`.

Como todos los problemas complejos, comenza por dividirlo en problemas mas pequeños: por ejemplo, comenza por una funcion que devuelva un numero aleatorio. Una vez que la tengas, hacé una función que reciba un array y devuelva un número aleatorio en cada posición de ese array. Luego, mejorala para hacer que devuelva un array cuyos elementos sean elementos aleatorios del array recibido como parametro. Solo entonces, hace la funcion generarGrilla. 

```javascript
generarGrilla(2, 3, [1, 2]) /* 
  [
    [1, 1, 2], 
    [2, 1, 1]
  ]
*/

generarGrilla(3, 3, ['a', 'b', 'c']) /* 
  [
    ['c', 'c', 'a'], 
    ['c', 'a', 'a'], 
    ['b', 'a', 'b']
  ]
*/
```

### 8 `generarMatrizEscalonada(filas)`

Crear una función `generarMatrizEscalonada` que tome como argumento un número entero `filas` y devuelva un array 2d con la cantidad de filas `filas`, donde la primera fila tiene 1 columna, la segunda tiene 2, la tercera 3, y así sucesivamente. Los ítems de la matriz deben ser `0`.

```javascript
generarMatrizEscalonada(3) /* 
  [
    [0], 
    [0, 0], 
    [0, 0, 0]
  ] */
generarMatrizEscalonada(5) /* 
  [
    [0], 
    [0, 0], 
    [0, 0, 0], 
    [0, 0, 0, 0], 
    [0, 0, 0, 0, 0]
  ] */
```
