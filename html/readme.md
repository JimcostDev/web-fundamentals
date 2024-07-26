# Historia de la Web y Nacimiento de HTML

## Introducción a la Historia de la Web

### 1. Orígenes de Internet
- **Años 1960-1970**: Desarrollo de ARPANET, una red de computadoras creada por el Departamento de Defensa de los Estados Unidos para la comunicación entre diferentes redes.
- **1980s**: Evolución de ARPANET y la creación de protocolos como TCP/IP que permiten la interconexión de redes múltiples.

### 2. Tim Berners-Lee y el Nacimiento de la Web
- **1989**: Tim Berners-Lee, un científico informático del CERN (Organización Europea para la Investigación Nuclear), propone un proyecto de hipertexto para facilitar el intercambio de información entre investigadores.
- **1990**: Desarrollo de las primeras tecnologías web: HTML (HyperText Markup Language), HTTP (HyperText Transfer Protocol) y un navegador/editor llamado WorldWideWeb.

## ¿Qué es HTML?
HTML (Lenguaje de Marcas de Hipertexto, del inglés HyperText Markup Language) es el componente más básico de la Web. Define el significado y la estructura del contenido web.  HTML utiliza una estructura basada en etiquetas (tags) para definir elementos como párrafos, encabezados, enlaces, imágenes y otros tipos de contenido.

## El Significado del Nombre
- **HyperText**: Se refiere a la capacidad de HTML para crear enlaces entre diferentes páginas web o entre diferentes partes de la misma página. Estos enlaces son conocidos como hipervínculos, y permiten la navegación no lineal, es decir, los usuarios pueden saltar de un documento a otro fácilmente.
- **Markup Language**: Indica que HTML es un lenguaje de marcado, lo que significa que utiliza etiquetas para marcar y definir el contenido de un documento. A diferencia de los lenguajes de programación, los lenguajes de marcado no realizan cálculos ni ejecutan acciones, sino que organizan y estructuran el contenido.


## Evolución de HTML

### HTML 1.0
- **1993**: Primer lanzamiento oficial de HTML, definido por Tim Berners-Lee. Soporta texto, hipervínculos y pocas etiquetas básicas.

### HTML 2.0
- **1995**: Publicado por el IETF (Internet Engineering Task Force), estandariza y mejora HTML 1.0, incluyendo formularios y otras funcionalidades básicas.

### HTML 3.2 y HTML 4.0
- **1997-1999**: Lanzamientos que introducen más etiquetas y atributos, mejor soporte para scripts y estilos, y comienzan a separar la estructura del contenido y la presentación (con la ayuda de CSS).

### XHTML
- **2000**: Transición hacia un lenguaje más estricto y basado en XML. Busca mayor rigor en la sintaxis del código HTML.

### HTML5
- **2014**: La versión más reciente y robusta de HTML, desarrollada por el W3C y WHATWG. Introduce numerosas mejoras:
  - Nuevos elementos semánticos como `<article>`, `<section>`, `<nav>`, y `<footer>`.
  - Soporte mejorado para multimedia con etiquetas `<audio>` y `<video>`.
  - API y elementos para aplicaciones web más interactivas y dinámicas.



## Conclusión
HTML no es un lenguaje de programación; es un lenguaje de marcado que define la estructura de tu contenido. HTML consiste en una serie de elementos que usarás para encerrar diferentes partes del contenido para que se vean o comporten de una determinada manera. 


---
 
# Fundamentos de HTML

## Anatomía de un elemento HTML

![img-anatomia-html-mdn](https://developer.mozilla.org/es/docs/Learn/Getting_started_with_the_web/HTML_basics/grumpy-cat-small.png)
```html
<p>Hola, estoy aprendiendo sobre desarrollo web.</p>
```

## Anidar elementos
Puedes también colocar elementos dentro de otros elementos —esto se llama anidamiento—.
```html
<p>Hola, estoy aprendiendo sobre <strong>desarrollo web</strong>.</p>
```

## Elementos vacíos
Algunos elementos no poseen contenido, y son llamados **elementos vacíos**.

```html
<img src="https://www.jimcostdev.com/dev.webp" alt="Mi imagen de prueba" />
```
## Anatomía de un documento HTML (estructura base)
Hasta ahora has visto lo básico de elementos HTML individuales, pero estos no son muy útiles por sí solos. Ahora verás cómo los elementos individuales son combinados para formar una página HTML entera.

```html
<!doctype html>
<html>
  <head>
    <meta charset="utf-8" />
    <title> Mi pagina de prueba</title>
    <link rel="icon" type="image/webp" href="/logo.webp" />
    <meta name="description" content="¡Hola! Soy Ronaldo Jiménez, un Software Developer apasionado por la creación de soluciones tecnológicas. Descubre mi experiencia laboral, educación y más.">
    <meta name="keywords" content="Ronaldo Jiménez, Web Developer, Desarrollador web, jimcostdev, Python">
    <meta name="author" content="Ronaldo Jiménez">
    <!--Open Graph (integrar la página web con redes sociales.) -->
    <meta property="og:title" content="JimcostDev by Ronaldo Jiménez | Software Developer">
    <meta property="og:description" content="¡Hola! aqui va mi super descripción">
    <meta property="og:image" content="https://user-images.githubusercontent.com/53100460/254561844-6471bed7-ba32-4d66-b05f-007da9a95620.jpg">
    <meta property="og:url" content="https://www.jimcostdev.com/">
  </head>
  <body>
    <img src="https://www.jimcostdev.com/dev.webp" alt="Mi imagen de prueba" />
  </body>
</html>
```

## Marcado de texto

### Encabezados
Los elementos de encabezado permiten especificar que ciertas partes del contenido son encabezados, o subencabezados del contenido. De la misma forma que un libro tiene un título principal, y que a su vez puede tener títulos por cada capítulo individual, y subtítulos dentro de ellos, un documento HTML puede tenerlos también.

```html
<h1>Mi título principal</h1>
<h2>Mi título de nivel superior</h2>
<h3>Mi subtítulo</h3>
<h4>Mi sub-subtítulo</h4>
```

### Párrafos
Como se explicó más arriba, los elementos **```<p>```** se utilizan para encerrar párrafos de texto; los usarás frecuentemente para el marcado de contenido de texto regular:
```html
<p>Este es un parrafo</p>
```

### Listas
Los dos tipos de listas más comunes son las listas ordenadas y las desordenadas:

1. **Las listas desordenadas** son aquellas en las que el orden de los items no es relevante, como en una lista de compras. Estas son encerradas en un elemento ```<ul>``` (unordered list).
   
2. **Las listas ordenadas** son aquellas en las que el orden sí es relevante, como en una receta. Estas son encerradas en un elemento ```<ol>``` (ordered list).

Por ejemplo:
```html
<p>Mis skills técnicas son:</p>

<ul>
  <li>Python</li>
  <li>React</li>
  <li>MongoDB</li>
</ul>

<p>Mucho más...</p>

```

### Vínculos
Los vínculos o enlaces son muy importantes —son los que hacen de la web, la web—. Para implementar un vínculo, necesitas usar un vínculo simple — ```<a>``` — la a es la abreviatura de la palabra inglesa «anchor» («ancla»). 
```html
<a href="https://developer.mozilla.org/es/docs/Learn/Getting_started_with_the_web/HTML_basics"> Conceptos básicos de HTML </a>
```

Tomado de: [Conceptos básicos de HTML](https://developer.mozilla.org/es/docs/Learn/Getting_started_with_the_web/HTML_basics)