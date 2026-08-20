#comandos 

Para sabe la shell que se está ejecutando en nuestra terminal existen varios métodos. El primero es con el comando __ps__.

## ps

ps sirve para ver los procesos que se están ejecutando. ps (processes)

## echo

el comando echo hace referencia a su nombre, hace eco, repite texto. Otra funicón es que te pemite sabe información sin importar en que directorio se encuentra. Por ejemplo, para ver el shell que se está utilizando se puede usar echo $SHELL.

## date

Como su nombre lo indica este comando te muestra la fecha y hora actual. Hay variantes que se pueden aplicar al comando date, utilizando modificadores (argumentos) como +%Y, +%D o +%s

## cd

Change directory se usa para cambiar el directorio desde el que se está trabajando.  cd debe ir acompañado por un argumento, este argumento puede ser un path absoluto o un path relativo. Si se llama a cd sin ningún argumento, por default te llevará al directorio home.  cd .. te lleva al parent directory, el directorio que está un nivel arriba. cd . no te lleva a ningún lado, el (.) se refiere al directorio actual. 

##  ls

Te muestra una lista de todos los archivos y directorios que se encuentran en el directorio en el que se encuentra. ls -a (all) te muestra todos los archivos, incluso los que están ocultos. ls -r invierte el orden alfabético de la lista. ls -t  cambia la lista del archivo más reciente al más antiguo.  Se pueden combinar argumentos y poner ls -tr y mostrará una lista donde se acomode primero los archivos más antiguos al princio y los más viejos al final. 

## Cat  / Head / Tail / Less

La función de este comandoi es mostrar el contenido de los archivos. Cuando un archivo es muy grande se desplegará todo en la terminal y no podra ser visible en la ventana. Hay dos variantes de este comando que te pueden servir para desplegar solo una parte del contenido del archivo. 

__head__ te muestra las primeras 10 lineas de un archivo, puede asignarsele un argumento para determinar el número de líneas que se desea mostrar. Ejemplo:

```bash
elato ~% head -5 switch-desk-sh
#!/bin/bash

if [ -z "$1" ]; then
  echo "Usage: $0 1|2|3"
  exit 1
```

__Tail__  funciona de la misma forma, pero con las últimas líneas del archivo. Ejemplo:

```bash
elato ~% tail -5 switch-desk-sh
gsettings set org.cinnamon.desktop.background picture-uri "file://$IMG"

# Set Cinnamon background (file URI)
gsettings set org.cinnamon.desktop.background picture-uri "file://$IMG"

```

__less__ es un  comando que te permite leer archivos en la ventana de la terminal, lo que hace es desplegar el texto solo hasta llenar la pantalla, para continuar se puede precionar la tecla espacio o b para regresar. Una vez que se haya terminado se preciona la tecla q parra salir del comando. 

## df

Este comando te muestra información sobre tui disco duro. Hay una variante df -h(human friendly) que te muestra la información de una manera más legible para los usuarios comunes. 

## uptime

Este comando te muestra informacion acerca del tiempo que tiene activo el sistema. Ejemplo:

```Bash
elato ~ % uptime
16:16:58 up 6:23, 1 user, load average: 0.40, 0.54, 0.75

```

En  primer lugar aparece la hora en la que el comando es llamado,. seguido por el tiempo que lleva el sistema encendido desde el último reboot, el número de usuarios que se encuentran conectados y los tiempos de carga en 1 min, 5 min, 15 min. Entre menor sea el número menos ocupado se encuentra el procesador de la máquina.

## hostname / uname

hostname te muestra el nombre del usuario de la pc. uname te muestra el nombre de la unix que se está corriendo. Ejemplos:

```bash

elato@elato-iMac ~/Desktop/Obsidian/Git
 % hostname
elato-iMac
elato@elato-iMac ~/Desktop/Obsidian/Git
 % uname
Linux
```

uname cuenta con una variante uname -a que te arroja información más detalladda sobre el sistema. Ejemplo:

```bash
elato@elato-iMac ~ % uname -a
Linux elato-iMac 7.0.0-29-generic #29~24.04.2-Ubuntu SMP PREEMPT_DYNAMIC Wed Aug 12 17:25:56 UTC 2 x86_64 x86_64 x86_64 GNU/Linux
```

Se despliega el sistema operativo, el nombre del equipo, el kernel, cuandpo se hizo la modificación del kernel, la distribución, la arquitectura, etc.

## top

Este comando muestra todos los procesos que se están realizando en primer y segundo plano. 

## kill

Este comando se utiliza para detener procesos que se estén ejecutando. Se debe introducir el comando __kill__ seguido del PID (process ID). Para conocer el PID de un proceso se puede ejecutar el comando ps o el comando top, el PID será la primera columna de la izquierda.





______
 
[[Command Line Interface]]
