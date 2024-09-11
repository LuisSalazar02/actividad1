# Manual de uso paint.py

## Descripción de Funciones

### `rectangle(start, end)`

Esta función dibuja un rectángulo utilizando la biblioteca de gráficos de tortuga (turtle). El rectángulo se define por los puntos `start` y `end`, que representan dos esquinas opuestas del mismo.

- **Parámetros**:
  - `start`: Un objeto punto que define una esquina del rectángulo. Debe tener atributos `x` y `y` que representan las coordenadas.
  - `end`: Un objeto punto que define la esquina opuesta del rectángulo, también con atributos `x` y `y`.
- **Funcionalidad**:
  - La tortuga se mueve al punto `start` y se llama a la función `begin_fill()` para llenar el rectángulo con color.
  - La tortuga dibuja el rectángulo alternando entre el ancho (diferencia entre `start.x` y `end.x`) y la mitad de la altura del rectángulo.
  - La función `end_fill()` se usa para llenar el rectángulo.

### `triangle(start, end)`

Esta función dibuja un triángulo equilátero desde el punto `start`, con cada lado de longitud definida por la diferencia entre `end.x` y `start.x`.

- **Parámetros**:
  - `start`: Un objeto punto que define el vértice inicial del triángulo.
  - `end`: Un objeto punto utilizado para calcular la longitud del lado del triángulo. Debe tener atributos `x` y `y`.
- **Funcionalidad**:
  - La tortuga se mueve al punto `start` y se llama a la función `begin_fill()` para llenar el triángulo con color.
  - Luego, la tortuga dibuja un triángulo equilátero moviéndose hacia adelante con la longitud de `end.x - start.x` y girando 120 grados después de cada lado.
  - La función `end_fill()` se usa para llenar el triángulo.
