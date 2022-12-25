  Vamos a ir viendo las propiedades que podemos aplicar sobre los grid items:

- grid-column ( grid-column-start + grid-column-end) / grid-row (grid-row-start + grid-row-end)
- grid-area
- place-self (align-self / justify-self)

### GRID-COLUMN / GRID ROW

**grid-column** y **grid-row** son una combinación de:

 
```css
.item {
  grid-column-start: 1;
  grid-column-end: span 2;
}

/* en una sola propiedad */

.item{
  grid-column: 1 / span 2;
}
```

 

Nos ayuda a definir el tamaño de cada item. Por ejemplo para el ejercicio anterior:

```css
.container{
  display: grid;
  width: 400px;
  height: 400px;
  background-color: pink;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr;
}

.item-1{
  grid-column: 1 / span 3;
  grid-row: 1 / span 1;
  background-color: blue;
}
.item-2{
  grid-column: 1 / span 1;
  grid-row: 2 / span 1;
  background-color: yellow;
}
.item-3{
  grid-column: 3 / span 1;
  grid-row: 2 / span 1;
  background-color: green;
}
.item-4{
  grid-column: 1 / span 3;
  grid-row: 3 / span 1;
  background-color: red;
}
```

### **GRID-AREA**

Tenemos dos valores con los que podemos trabajar el **grid-area**

 

```css
.item {
  grid-area: item-1; /* usamos para definir el nombre del item a usar en el grid-template-areas */
}

/* en una sola propiedad */

.item{
  grid-area: 3 / 3 / span 1 / span 1; /* row-start / column-start / row-end / column-end */
}
```

 

### **PLACE-SELF**

Nos sirve para posicionar el elemento dentro de la cuadrícula de forma única:

```css
.item {
  align-self: center; /* vertical */
  justify-self: center;	/* horizontal */
}

/* en una sola propiedad */

.item{
  place-self: center center; /* align-self justify-self */
}
```
