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


### POR CORTE DE LUZ

Dejamos algunos ejercicios optativos de arrays para quienes quieran seguir practicando. 

Como alternativa, les recomiendo que revean las clases 38 y 39 en donde hablamos de arrays y matrices. Si se sienten confiadas, pueden intentar los ejercicios 3 y 4 luego de verlas. 

### `sumarSeccion(array, comienzo, cantidad)`

Crear una función `sumarSeccion` que tome como argumento un array de números enteros `array`, un número entero `comienzo` y un número entero `cantidad`, y que devuelva la suma de `cantidad` de números de `array` empezando a contar desde el ítem con índice `comienzo`.

```javascript
sumarSeccion([2, 2, 4, 3, 10, 20, 5], 0, 3) // 8 (2 + 2 + 4 = 8)
sumarSeccion([2, 2, 4, 3, 10, 20, 5], 2, 4) // 37 (4 + 8 + 10 + 20 = 37)
sumarSeccion([2, 2, 4, 3, 10, 20, 5], 4, 1) // 3
```

### `esSubconjunto(subconjunto, conjunto)`

Crear una función `esSubconjunto` que tome como argumento dos arrays, `subconjunto` y `conjunto`, y devuelva `true` si `subconjunto` es realmente subconjunto de `conjunto`, es decir, si todos los valores de `subconjunto` están en `conjunto`.

```javascript
esSubconjunto([1], [1, 2, 3]) // true
esSubconjunto([1, 2, 3], [1, 2, 3, 4, 5]) // true
esSubconjunto([27, 49, 54], [54, 27, 8, 27, 49]) // true
esSubconjunto([1, 2, 3], [1, 2]) // false
esSubconjunto([1], [2, 3, 4]) // false
```

### `tieneBloque(array)`

Crear una función `hayBloque` que tome como argumento un array `array` y devuelva `true` si dicho `array` tiene un bloque de 3 o más ítems consecutivos idénticos, o `false` si no tiene.

```javascript
tieneBloque([1, 2, 3]) // false
tieneBloque([1, 1, 1, 2, 3]) // true
tieneBloque([1, 2, 3, 3, 3]) // true
tieneBloque([1, 2, 3, 3, 3, 8]) // true
tieneBloque([1, 2, 2, 3, 3, 4]) // false
```

 
### CONTINUAREMOS EL MIERCOLES 4/4 CON LOS SIGUIENTES EJERCICIOS 

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
