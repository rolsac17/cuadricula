# cuadricula

Manejo de cuadricula

## Notas

- _Grid Container_
  Elemento padre donde se asigna un (display: grid;).

- _Grid Item_
  Hijos directos de un grid container.

```html
<div class="container">
  <div class="item"></div>

  <div class="item">
    <p class="sub-item"></p>
  </div>

  <div class="item"></div>
</div>
```

Los grid item unicamente son los item ya que son hijos directos del grid
container, mientras que el sub-item que aparece no lo es ya que su padre directo
es un grid item.

- _Grid Line_
  Lineas divisoras horizontales y verticales de la cuadricula.

- _Grid Track_
  Espacio entre dos lineas adyacentes, mejor conosidos como: filas y columnas.

- _Grid Cell_
  Espacio en dos filas adyacentes y dos columnas adyacentes.

- _Grid Area_
  Espacio rodeado por cuatro grid lines.
