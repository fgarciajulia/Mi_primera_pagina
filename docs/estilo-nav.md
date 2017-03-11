# Colocamos estilo al menú

Para añadir estilo al menú vamos a ir a nuestro archivo main.css y añadimos lo siguiente:


```
.navbar-custom {
    background: #2C3E50;
    font-family: "Montserrat", "Helvetica Neue", Helvetica, Arial, sans-serif;
    text-transform: uppercase;
    font-weight: 700;
    border: none;
}

.navbar-custom a:focus {
    outline: none;
}

.navbar-custom .navbar-brand {
    color: white;
}

.navbar-custom .navbar-brand:hover,
.navbar-custom .navbar-brand:focus,
.navbar-custom .navbar-brand:active,
.navbar-custom .navbar-brand.active {
    color: white;
}

.navbar-custom .navbar-nav {
    letter-spacing: 1px;
}

.navbar-custom .navbar-nav li a {
    color: white;
}

.navbar-custom .navbar-nav li a:hover {
    color: #18BC9C;
    outline: none;
}

.navbar-custom .navbar-nav li a:focus,
.navbar-custom .navbar-nav li a:active {
    color: white;
}

.navbar-custom .navbar-nav li.active a {
    color: white;
    background: #18BC9C;
}

.navbar-custom .navbar-nav li.active a:hover,
.navbar-custom .navbar-nav li.active a:focus,
.navbar-custom .navbar-nav li.active a:active {
    color: white;
    background: #18BC9C;
}

.navbar-custom .navbar-toggle {
    color: white;
    text-transform: uppercase;
    font-size: 10px;
    border-color: white;
}

.navbar-custom .navbar-toggle:hover,
.navbar-custom .navbar-toggle:focus {
    background-color: #18BC9C;
    color: white;
    border-color: #18BC9C;
}

@media (min-width: 768px) {
    .navbar-custom {
        padding: 25px 0;
        -webkit-transition: padding 0.3s;
        -moz-transition: padding 0.3s;
        transition: padding 0.3s;
    }
    .navbar-custom .navbar-brand {
        font-size: 2em;
        -webkit-transition: all 0.3s;
        -moz-transition: all 0.3s;
        transition: all 0.3s;
    }
    .navbar-custom.affix {
        padding: 10px 0;
    }
    .navbar-custom.affix .navbar-brand {
        font-size: 1.5em;
    }
}
```

Si abrimos el index.html en nuestro navegador deberiamos ver algo así:

![Imagen](https://fgarciajulia.github.io/mi_primera_pagina/img/menu1.jpg)


## ¿Que fue lo que hicimos?

Añadimos estilos al menú, entre ellos:

- Colores.
- Márgenes internos.
- Bordes de color.
- Márgenes externos.
- Elegimos una familia tipografica, les dijimos que grosor deben tener, que interletrado.
- Le dijimos que haya textos que se pongan en mayúscula
- Variaciones de tamaño
- Tiempos de transición para estas variaciones de tamaño.

y algunas cosas más...

> Por ahi apareció un **@media**, la funcion que cumple es decir "todo lo que esta acá adentro, solo aplica **sí** la pantalla tiene" y luego viene la condición que dice **(min-width: 768px)** "un ancho minimo de 768px".

## Selectores

Para crear diseños web profesionales, es imprescindible conocer y dominar los selectores de CSS. Como se vio en el capítulo anterior, una regla de CSS está formada por una parte llamada "selector" y otra parte llamada "declaración".

La declaración indica "qué hay que hacer" y el selector indica "a quién hay que hacérselo". Por lo tanto, los selectores son imprescindibles para aplicar de forma correcta los estilos CSS en una página.

A un mismo elemento HTML se le pueden aplicar varias reglas CSS y cada regla CSS puede aplicarse a un número ilimitado de elementos. En otras palabras, una misma regla puede aplicarse sobre varios selectores y un mismo selector se puede utilizar en varias reglas.

El estándar de CSS 2.1 incluye una docena de tipos diferentes de selectores, que permiten seleccionar de forma muy precisa elementos individuales o conjuntos de elementos dentro de una página web.

No obstante, la mayoría de páginas de los sitios web se pueden diseñar utilizando solamente los cinco selectores básicos.

## Recomendación:

Te recomiendo FUERTEMENTE que si te costo entender el código que escribimos anteriormente visites esta página donde explican muy bien este tema.<br />
De lo contrario TAMBIEN hechale un vistaso a los selectores avanzados, porque hay selectores que no suelen usarse mucho pero cuando los necesitas, son irremplazable, solo hay que saber que excisten, y a la hora de necesitarlos investigaras como se escriben.

[Selectores basicos](https://librosweb.es/libro/css/capitulo_2/selectores_basicos.html)<br />
[Selectores avanzados](http://librosweb.es/libro/css/capitulo_2/selectores_avanzados.html)