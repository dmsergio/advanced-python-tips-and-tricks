
# Deques

La mayor ventaja de este tipo de objetos es la eficiencia a la hora de agregar o quitar elementos. Con una lista también se podrían realizar este tipo de operaciones, pero penalizando en eficiencia.

## Importación

```python
from collections import deque
```

## Ejemplos

Declaración con 10 elementos, y además especificando un tamaño fijo de 10 elementos. Esto quiere que por mucho que se vayan agregando más elementos, el tamaño del contenedor se mandendrá fijo.

```python
dq = deque(range(10), maxlen=10)
```

Rotar cuatro posiciones a la derecha cada uno de los elementos

```python
dq.rotate(4) 
```

Rotar cuatro posiciones a la izquierda cada uno de los elementos

```python
dq.rotate(-4)
```

Agregar un nuevo elemento al comienzo (saca el último, al exceder el tamaño máximo)

```python
dq.appendleft(-1)
```

Agregar un array de elementos al final de la lista

```python
dq.extend([9, 10, 11, 12]) 
```

Agregar un array al comienzo de la lista

```python
dq.extendleft([2, 1])
```
