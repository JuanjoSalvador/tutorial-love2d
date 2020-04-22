## Introducción a Love2D

## ¿Qué es Love2D?

* Motor de videojuegos basado en Lua

* Por debajo corre SDL

* Nació en 2008

* Está escrito en C++

* Ligero y multiplataforma, puede correrese sobre una Raspberry Pi

* Gran comunidad (foros, blogs, etc)

* Buena documentación (tutoriales, wiki, vídeos)

* Licencia zlib

## Funciones básicas

* Como otros motores, se basa en el sistema iniciar-actualizar-dibujar.

* Función `love.load()`

    * Inicializa el juego, es la primera función que se llama siempre, carga los módulos necesarios e inicializa las variables requeridas. 

    * Se llama una vez solamente.

* Función `love.update()`

    * Actualiza las variables y los estados del juego

    * Se llama hasta 60 veces por segundo

    * Aquí se sitúa el funcionamiento del juego

* Función `love.draw()`

    * Dibuja los gráficos de nuestro juego

    * Se llama hasta 60 veces por segundo


## Extensible 

### Librerías

* Multitud de librerías e integraciones, desde detección de colisiones hasta animaciones e integraciones con software de terceros.

* Librerías que extienden Love2D para funcionar también como un motor grafico tridimensional (Löve3D)

* Shaders mediante OpenGL y C.

### Controles

* Soporta teclado y ratón

* Soporta gamepad

* Soporte para Xbox Controller

### API Lua-C

* Una de las ventajas de Lua es que es extensible mediante funciones en C

* Si necesitas escribir una función compleja o que no se encuentra en el API de Lua 5.1, puedes escribirla en C y cargarla en tu programa

## Herramientas

* El IDE "oficial" es ZeroBrane Studio, un IDE de Lua con multitud de funciones aplicables a este desarrollo.

* Love2D se puede integrar con la mayoría de editores famosos, ejemplo: Emacs, VS Code, Vim, Atom, etc.

* Soporta integración con Tiled (herramienta para crear mapas basados en tilesets, o mosaicos) mediante la librería STI.