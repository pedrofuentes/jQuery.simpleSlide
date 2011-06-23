jQuery SimpleSlide
=============

A simple slide jQuery plugin.

Chek the [original post](http://pedrofuent.es/2009/08/transicion-de-imagenes-o-slideshow-con-jquery/)

Overview
-------

The markup of your accordion container needs the images and a content panel

    <div id="container">
        <img src="imagen_1.jpg" alt="Imagen 1" />
        <img src="imagen_2.jpg" alt="Imagen 2" />
        <img src="imagen_3.jpg" alt="Imagen 3" />
        <img src="imagen_4.jpg" alt="Imagen 4" />
        <img src="imagen_5.jpg" alt="Imagen 5" />
    </div>

And then just apply the plugin to the container

    $(document).ready(function(){
 
        $("#contenedor").simpleSlide();
 
    });

If you use a different element than images, for example if you are adding links

    <div id="container">
        <a href="#1"><img src="imagen_1.jpg" alt="Imagen 1" /></a>
        <a href="#2"><img src="imagen_2.jpg" alt="Imagen 2" /></a>
        <a href="#3"><img src="imagen_3.jpg" alt="Imagen 3" /></a>
        <a href="#4"><img src="imagen_4.jpg" alt="Imagen 4" /></a>
        <a href="#5"><img src="imagen_5.jpg" alt="Imagen 5" /></a>
    </div>

Specify the element option

    $(document).ready(function(){

        $("#contenedor").simpleSlide({element:'a'});

    });

Options
-------

* duration

    Set the time that will take to move to the next element

* transition

    Set the time that the fade between elements will take

* stopAt

    Set a limited amount of transitions

* element

    Set the element

Copyright
------------

    Copyright (c) 2010 Pedro Fuentes ( http://pedrofuent.es )
    Dual licensed under the MIT and GPL licenses:
    http://www.opensource.org/licenses/mit-license.php
    http://www.gnu.org/licenses/gpl.html