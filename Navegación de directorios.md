
En linux todo parte del root directory (/).  En el root directory encontraremos diferentes carpetas como:
- __bin__ (binaries) que hace referencia a programas o archivos ejecutables, es donde la computadora guarda los comandos mínimos y esenciales para que el sistema funcione.
- __etc__ (configuraciones)
- __home__ (donde se alojan los archivos personales del usuario, no relacionados con el funcionamiento del equipo)
- __tmp__ (archivos temporales)
- __usr__ (se guardan binaries que no están relacionadas con el funcionamiento del sistema) 
- __var__ (donde se almacenan archivos volátiles)

el path a un directorio comienza con un /, este es el directorio absoluto, un path relativo comienza sin el slash y hace referencia a un directorio que esté en el mismo path del directorio en el que nos encontremos. 

Para saber en que directorio te encuentras hay distintos modos de hacerlo, en primer lugar el directorio se muestra en el prompt:  [~ %] o [/home %].  Este método no siempre es completamente confiable, se puede configurar la shell para cambiar esto. Una forma de hacerlo fácil y confiable es con el comando __pwd__ (Print the Working Directory). Ejemplo: ~ % pwd: /home.

Para cambiar el directorio donde se encuentra la shell se utiliza el comando __cd__ [[Primeros comandos]]. La diferencia ente un path relativo y uno absoluto es que el absoluto te puede llevar a cualquier directorio sin importar la carpeta donde te encuentras. Para que un path sea absoluto se debe introducir todo el camino. 

