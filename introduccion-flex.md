El objetivo del módulo **Flexbox** es ofrecer una  forma más eficiente para poder alinear, diseñar y distribuir el espacio de los elementos dentro de un contenedor. Incluso en circunstancias donde su contenido es desconocido.

La idea principal detrás del diseño flexible es darle al contenedor la capacidad de modificar el ancho, alto y orden de los elementos para ocupar de una manera más óptima el espacio disponible y así poderse adaptar más eficientemente a los distintos tamaños de pantalla. Esta funcionalidad permite ampliar y reducir los tamaños de sus hijos para ir adaptándolos y evitar que desborden.

A diferencia de otros métodos, Flexbox nos permite trabajar controlando a la vez columnas y filas, esto sucede gracias a la distribución de elementos en dos ejes. Tendrán un eje principal y uno secundario:

- El flex-container tendrá una orientación principal específica (por defecto, filas)
- La orientación secundaria del flex-container será la perpendicular a la específica (si es filas será columnas y si es columnas será filas)

```html
<div class="flex-container">
    <div class="flex-item">Hijo flexible 1</div>
    <div class="flex-item">Hijo flexible 2</div>
    <div class="flex-item">Hijo flexible 3</div>
    <div class="flex-item">Hijo flexible 4</div>
</div>
```

```css
.flex-container{
	display:flex;
}
```

En el siguiente video veremos las propiedades del flex-container para empezar a aplicar toda esta información.