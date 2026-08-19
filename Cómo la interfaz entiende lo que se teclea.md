
Cuando se introduce texto en la terminal no sucede nada hasta que no se preciona return. Un comando es lo que se escribe en la terminal justo despúes del primer espacio.  Cuando se introduce un comando la interfaz lo que hace es buscar en el path para ver si encuentra un comando como el que se ha introducido. Este es mi PATH:

/home/elato/.local/bin:/home/elato/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin

La interfaz va por cada uno de estos directorios buscando si hay un comando como el que se le ha introducido.

Hay un comando que te permite saber donde se encuentran los comandos: type. Ejemplo: 

```bash

elato~% type cat
cat is /usr/bin/cat

```

Cada vez que se preciona enter la interfaz lee lo que se debe interpretar, los argumentos que se le agregan al comando, una vez que ha interpretado esos argumentos entonces ejecuta el comando. 

[[Command Line Interface]]