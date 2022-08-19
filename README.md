# 2C2022-162013G1
Bitácora de comandos para la clase de Sistemas Operativos.

Joshua Martínez Marchena.

Universidad Latinoamericana de Ciencia y Tecnología
ULACIT
2022

# Información del sistema

## 1- arch
muestra la arquitectura de la máquina (1).

## 2- uname -m
muestra la arquitectura de la máquina (2).

## 3- uname -r
muestra la versión del kernel usado.

## 4- dmidecode -q 
muestra los componentes de hardware del sistema.

## 5- hdparm -i /dev/hda: 
muestra las características de un disco duro.

## 6- hdparm -tT /dev/sda
realizar prueba de lectura en un disco duro.

## 7- cat /proc/cpuinfo
muestra la información del CPU.

## 8- cat /proc/interrupts
muestra las interrupciones.

## 9- cat /proc/meminfo
Verificación del uso de memoria.

## 10- cat /proc/swaps
muestra ficheros swap.

## 11- cat /proc/version
muestra la versión del kernel.

## 12- cat /proc/net/dev
muestra adaptadores de red y las estadísticas.

## 13- cat /proc/mounts
muestra el sistema de ficheros montado.

## 14- lspci -tv
muestra los dispositivos PCI.

## 15- lsusb -tv
muestra los dispositivos USB.

## 16- _date
muestra la fecha del sistema.

## 17- cal 2022 
encargado de mostar el almanaque de 2022 o año que se le indique.

## 18- cal 10 2022
muestra el almanaque para el mes octubre de 2022 o el que se le indique.

## 19- date 041217002011.00
coloca y declara, ajusta la fecha y hora.

## 20- clock -w
guarda los cambios de fecha en la BIOS.

# Reiniciar, apagar o cerrar sesion 

## 1- shutdown -h now 
apaga el sistema (1).

## 2- init 0
apaga el sistema (2).

## 3- telinit 0
apaga el sistema (3).

## 4- halt
apaga el sistema (4).

## 5- shutdown -h hours minutes &
apagado planificado del sistema.

## 6- shutdown -c 
cancela un apagado que ha sido planificado del sistema.

## 7- shutdown -r now
reiniciar (1).

## 8- reboot 
reiniciar (2).

## 9- logout
cerrar la sesión.

# Directorios y archivos.

## 1- cd /home
ingresar en el directorio “home”.

## 2- cd ..
retrocede un nivel.

## 3- cd ../..
retrocede 2 niveles.

## 4- cd
ir al directorio raíz.

## 5- cd ~user1
ir al directorio user1.

## 6- cd –
regresa al directorio anterior.

## 7- pwd
muestar el camino del directorio de trabajo.

## 8- ls
para ver los ficheros de un directorio.

## 9- ls -F
para ver los ficheros de un directorio.

## 10- ls -l
muestra los detalles de ficheros y las carpetas de un directorio.

## 11- ls -a
muestra los ficheros ocultos.

## 12- ls [0-9]
muestra los ficheros y las carpetas que contienen números.

## 13- tree
muestra los ficheros y carpetas en forma de árbol iniciando por la raíz.(1)
 
## 14- lstree
muestra los ficheros y carpetas en forma de árbol iniciando por la raíz.(2)

## 15- mkdir dir1
crear una carpeta o directorio con nombre ‘dir1’.

## 16- mkdir dir1 dir2
Creación de dos carpetas o directorios simultáneamente.

## 17- mkdir -p /tmp/dir1/dir2
crea un árbol de directorios.

## 18- rm -f file1
borra el fichero llamado ‘file1’.

## 19- rmdir dir1
borra la carpeta llamada ‘dir1’.

## 20- rm -rf dir1
elimina una carpeta llamada ‘dir1’ con su contenido de forma recursiva. 

## 21- rm -rf dir1 dir2
elimina dos carpetas (o directorios) con su contenido de forma recursiva.

## 22- mv dir1 new_dir
renombra o mueve un fichero o carpeta (directorio).

## 23- cp file1
copia un fichero.

## 24- cp file1 file2
copia dos ficheros al unísono.

## 25- cp dir /* .
copia todos los ficheros de un directorio dentro del directorio de trabajo actual.

## 26- cp -a /tmp/dir1 .
copia un directorio dentro del directorio actual de trabajo.

## 27- cp -a dir1
copia un directorio.

## 29- cp -a dir1 dir2
copia 2 directorio al unísono.

## 30- ln -s file1 lnk1
crea un enlace simbólico al fichero o al directorio.

## 31- ln file1 lnk1
crea un enlace físico al fichero o al directorio.

## 32- touch -t 0712250000 file1 
modifica el tiempo real de un fichero o directorio.

## 33- file file1
salida o volcado de pantalla del tipo mime de un fichero texto.

## 34- iconv -l
listas de cifrados ya conocidos.

# Encontrar Archivos.

## 1- find / -name file1
busca fichero y directorio a partir de la raíz del sistema.

## 2- find / -user user1
busca ficheros y directorios pertenecientes al usuario ‘user1’.

## 3- find /home/user1 -name *.bin
busca ficheros con extensión ‘. bin’ dentro del directorio ‘/ home/user1’.

## 4- find /usr/bin -type f -atime +100
busca ficheros binarios no utilizados en los últimos 100 días.

## 5- find /usr/bin -type f -mtime -10
busca ficheros creados o cambiados dentro de los últimos 10 días.

## 6- find / -name *.rpm -exec chmod 755 ‘{}’ ;
busca ficheros con extensión ‘.rpm’ y modificar permisos.


# Comandos Docker

## 1- build	
Construir una imagen a partir de un Dockerfile

## 2- history	
Mostrar el historial de una imagen

## 3- import	
Importar el contenido de una tarball para crear una imagen del sistema de archivos

## 4- inspect
Mostrar información detallada sobre una o más imágenes

## 5- load
Cargar una imagen de un archivo tar o STDIN

## 6- ls	
Listar imágenes

## 7- prune	
Eliminar imágenes no utilizadas

## 8- pull	
Extraer una imagen o un repositorio de un registro

## 9- push	
Empujar una imagen o un repositorio a un registro

## 10- rm	
Eliminar una o más imágenes

## 11- save	
Guardar una o más imágenes en un archivo tar 

## 12- tag	
Cree una etiqueta TARGET_IMAGE que haga referencia a SOURCE_IMAGE
