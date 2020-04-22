## Tu primer programa en Love2D

Dicho de otro, tu Hello World :-)

### Punto de entrada: main.lua

El punto de entrada de todo programa que ejecutamos en Love2D, siempre es el `main.lua`. Empezamos por ahí, creando un fichero nuevo donde escribiremos nuestro programa.

```lua
-- Hello Love!
function love.load()
end

function love.update()
end

function love.draw()
    -- Llamamos a la función love.graphics.print() para imprimir un mensaje en pantalla
    love.graphics.print("Hello World!" 100, 100)
end
```

Y lo ejecutamos. Si estás en Linux o macOS, mi recomendación es lanzarlo desde la terminal. Si estás en Windows, te aconsejo que añadas `love` al PATH, y lo lances desde una ventana de Powershell.

    love main.lua

Si todo va bien, veremos algo como esto:

![Hello World en Love2D](images/hello.png)

Más adelante, veremos cómo podemos además empaquetar nuestros juegos.

### Configuración: conf.lua

Además del `main.lua`, existe otro fichero importante en nuestros juegos, el de configuración. Aquí le indicaremos qué módulos cargar, por defecto todos, además de indicarle la configuración de pantalla, gráficos, y otros parámetros.

Ejemplo:

```lua
function love.conf(t)
    t.window.width = 800
    t.window.height = 600
end
```

Si añadimos este fichero a nuestro ejemplo, se iniciará con un tamaño de 800x600 píxeles.

Un listado completo de parámetros que podemos pasarle, lo tenemos disponible en la [wiki de Love2D](https://love2d.org/wiki/Config_Files).