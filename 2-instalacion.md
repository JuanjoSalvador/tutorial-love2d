## Instalación y preparación del entorno

El propio entorno de ejecución incluye todo lo necesario, es decir, no requiere ningún tipo de prerrequisito de software, incluyendo Lua y LuaJIT. Está disponible en Linux (la mayor parte de las distribuciones lo incluyen en sus repositorios).

### Windows y OS X

Solo hay que descargar el ejecutable de la [versión más reciente desde aquí](https://github.com/love2d/love/releases/), e instalar como si de cualquier otro paquete se tratase.

#### Windows Powershell

Para poder acceder a Love2D desde la consola de Windows, algo muy recomendado para tareas de depuación, primero deberemos añadir el directorio de instalación, por defecto `C:\Archivos de programa\Love`, en la PATH del sistema.

### Linux

#### Debian/Ubuntu

    $ sudo apt install love

#### Otras distribuciones

Si no se encuentra en los repositorios, puede instalarse mediante AppImage. En un futuro, también por Flatpak.