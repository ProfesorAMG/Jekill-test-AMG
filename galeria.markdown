---
layout: page
title: Galería de imágenes
permalink: /Galeria/
---

¡Hola amigo!

<p>Si has llegado hasta aquí es porque querías ver las maravillosas imágenes de la carpeta images. </p>
    **************************+**************
    ***   IMAGENES DE LA CARPETA IMAGES   ***
    *****************************************
    {% for image in site.static_files %}
  {% if image.path contains 'images/' %}
  <p> Imagen </p>
    ![Descripción de la imagen]( {{ site.baseurl }}{{ image.path }} )
  {% endif %}
{% endfor %}
