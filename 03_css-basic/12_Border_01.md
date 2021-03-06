# Border

El **"concepto"** de border esta dividido en varias propiedades del tipo:
* `border-top-width:`
* `border-bottom-style:`
* `border-left-color:`

Entonces existen 4 **"parametros"** para definir un borde:
* `color`
* `width` (grosor)
* `style` (tipo)
* `posicion` (top, left,...)

Sobre la posicion se pueden usar los mismos principios usados en `margin` y `padding` (comenzar arriba, moverse en sentido horario, etc).

Entonces:
* `border-color: green;`
* `border-style: solid dashed;`
* `border-width: 3px 5px 2px;`

Valores de `border-style`:
* `solid`
* `dashed`
* `dotted`
* `double`
* `ridge`
* `inset`
* `outset`

```css
[class^="border"] {
  background: yellow;
  height: 50px;
  margin-bottom: 2em;
}

.border-1 {
  border-color: green red blue;
  border-style: solid dashed;
  border-width: 3px 5px 2px;
}
```

[Volver al inicio](#-Border)

## SHORTHAND

---------------------------------------------------------------------------

Existen **shortand** para cada posicion:
* `border-top:     width style color`
* `border-bottom:  width style color`
* `border-left:    width style color`
* `border-right:   width style color`

Sus valores: `width style color`

```css
.border-2 {
  border-top: 2px solid red;
  border-bottom: 3px dashed green;
}
```

> **NOTA**: El shorthand border se aplica a los cuatro lados, `border: width style color;`.

[Volver al inicio](#-Border)

## BORDER RADIUS

---------------------------------------------------------------------------

Forma individual:

* `border-bottom-left-radius: x y;`
* `border-bottom-right-radius: x y;`

> **NOTA**: El valor de `x` es el radio en horizontal.
> **NOTA**: El valor de `y` es el radio en vertical.
> **NOTA**: Si se indica un solo valor es para `x` e `y`.

El **shorthand** `border-radius` funciona igual que el de el margin para las posiciones. Con la diferencia de que se empieza a contar en la esquina superior izquierda.

Si se quiere definir el radio en `x` e `y` en el **shorthand** se debe separar con un slash (`/`). Así: `border-radius: valoresX / valoresY;`

```css
.border-3 {
  /*border-top-left-radius: 50%;*/
  /*border-radius: 50%;*/
  /*border-radius: 10px 30px;*/
  border-radius: 10px 20px / 20px;
  border: 1px solid black;
}
```

[Volver al inicio](#-Border)

## OUTLINE

---------------------------------------------------------------------------

Un `outline` (contorno) es una línea que se dibuja alrededor de los elementos, FUERA de los bordes, para hacer que el elemento "`stand out`".

CSS tiene las siguientes propiedades de esquema:
* `outline-style`
* `outline-color`
* `outline-width`
* `outline-offset`
* `outline`

> **NOTA**: `outline` se trataría igual que border.