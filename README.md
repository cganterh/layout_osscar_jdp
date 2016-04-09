# Layout para OSscar Jdp

Esta es la respuesta para una pregunta de OSscar Jdp en [Programadores Chile](https://www.facebook.com/groups/Programadores.Chile) sobre cómo hacer un layout en HTML.

En su pregunta, OSscar especifica que el layout debe verse de la siguiente manera:

![Imagen que especifica con lineas negras la forma que tiene que tener el layout.](requerimientos.jpg)

Se propone la siguiente solución:

<!DOCTYPE html>

<meta charset="utf-8">
<meta name="author" content="Cristóbal Ganter">

<title>Layout para OSscar Jdp</title>

<style>
    * {
        box-sizing: border-box;
    }

    header,
    div {
        border: 1px solid black;
        text-align: center;
    }

    header .izquierda,
    header .derecha {
        display: inline-block;
        vertical-align: middle;
        width: 50%;
    }

    .columna {
        display: inline-block;
        height: 66vh;
        vertical-align: top;
    }

    .columna.izquierda,
    .columna.derecha{
        width: 25%;
    }

    .columna.contenido {
        width: 50%;
    }
</style>

<header>
    <div class="superior">
        Superior
    </div><div class="izquierda">
        Inferior Izquierdo
    </div><div class="derecha">
        Inferior Derecho
    </div>
</header>

<div class="columna izquierda">
    Columna Izquierda
</div><div class="columna contenido">
    Contenido
</div><div class="columna derecha">
    Columna Derecha
</div>

Debe notarse que la solución propuesta no usa "flexbox" debido a la complejidad de esta tecnología para un principiante.
