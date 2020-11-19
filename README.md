# cuadricula

Manejo de cuadricula

## Notas

### Conseptos basicos

- **Grid Container**  
  Elemento padre donde se asigna un (display: grid;).

- **Grid Item**  
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

- **Grid Line**  
  Lineas divisoras horizontales y verticales de la cuadricula.

- **Grid Track**  
  Espacio entre dos lineas adyacentes, mejor conosidos como: filas y columnas.

- **Grid Cell**  
  Espacio en dos filas adyacentes y dos columnas adyacentes.

- **Grid Area**  
  Espacio rodeado por cuatro grid lines.

### Definicion de columnas

Nota de atajo:

```

  .item{contenido #$}*12

```

lo que hace el emet es crear 12 divs con contenido y la clase item.

- **grid-template-columns**  
  con el podemos definir las columnas de nuestra cuadricula, en cada 300px es una
  columna.

```css
.container {
  display: grid;
  grid-template-columns: 300px 300px 300px;
}
```

- **grid-template-rows**
  con el podemos definir las filas de nuestra cuadricula, cada unidad en pixeles
  indica las filas que necesitamos en este caso son tres.

```css
.container {
  display: grid;
  grid-template-rows: 300px 200px 100px;
}
```

```
Nota: por el momento solo estamos controlando el grid explicito de la cuadricula
pero tambien hay implicito que es, que ya viene por default.
```

Para una sintaxis mas corta donde se definen filas y columnas seria de la
siguiente forma:

```css
.container {
  display: grid;
  grid-template: 300px 200px 100px / 25% 50% 25%;
}
```

en el cual se piden primero las filas y luego las columnas
(grid-template: filas/columnas).

- **display: inline-grid**  
  lo que hace este display es que crea una cuadricula en linea todavia no disponible.
