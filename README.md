# 2C2022-162013G1
Bitácora de comandos para la clase de Sistemas Operativos.

Joshua Martínez Marchena.
Universidad Latinoamericana de Ciencia y Tecnología
ULACIT
2022

# Información del sistema

## arch
mostrar la arquitectura de la máquina (1).

## uname -m
mostrar la arquitectura de la máquina (2).

## uname -r
mostrar la versión del kernel usado.

## dmidecode -q 
mostrar los componentes (hardware) del sistema.

## hdparm -i /dev/hda: 
mostrar las características de un disco duro.

## hdparm -tT /dev/sda
realizar prueba de lectura en un disco duro.

## cat /proc/cpuinfo
mostrar información de la CPU.

## cat /proc/interrupts
mostrar las interrupciones.

## cat /proc/meminfo
verificar el uso de memoria.

## cat /proc/swaps
mostrar ficheros swap.

## cat /proc/version
mostrar la versión del kernel.

## cat /proc/net/dev
mostrar adaptadores de red y estadísticas.

## cat /proc/mounts
mostrar el sistema de ficheros montado.

## lspci -tv
mostrar los dispositivos PCI.

## lsusb -tv
mostrar los dispositivos USB.

## _date
mostrar la fecha del sistema.

## cal 2022 
mostrar el almanaque de 2022.

## cal 10 2022
mostrar el almanaque para el mes octubre de 2022.

## date 041217002011.00
colocar (declarar, ajustar) fecha y hora.

## clock -w
guardar los cambios de fecha en la BIOS.

# Reiniciar, apagar o cerrar sesion 

## shutdown -h now 
apagar el sistema (1).

## init 0
apagar el sistema (2).

## telinit 0
apagar el sistema (3).

## halt
apagar el sistema (4).

## shutdown -h hours minutes &
apagado planificado del sistema.

## shutdown -c 
cancelar un apagado planificado del sistema.

## shutdown -r now
reiniciar (1).

## reboot 
reiniciar (2).

## logout
cerrar sesión.

# Directorios y archivos.

## cd /home
entrar en el directorio “home”.

## cd ..
retroceder un nivel.

## cd ../..
retroceder 2 niveles.

## cd
ir al directorio raíz.

## cd ~user1
ir al directorio user1.

## cd –
regresar al directorio anterior.

## pwd
mostrar el camino del directorio de trabajo.

## ls
ver los ficheros de un directorio.

## ls -F
ver los ficheros de un directorio.

## ls -l
mostrar los detalles de ficheros y carpetas de un directorio.

## ls -a
mostrar los ficheros ocultos.

## ls [0-9]
mostrar los ficheros y carpetas que contienen números.

## tree
mostrar los ficheros y carpetas en forma de árbol comenzando por la raíz.(1)
 
## lstree
mostrar los ficheros y carpetas en forma de árbol comenzando por la raíz.(2)

## mkdir dir1
crear una carpeta o directorio con nombre ‘dir1’.

## mkdir dir1 dir2
crear dos carpetas o directorios simultáneamente (Crear dos directorios a la vez).

## mkdir -p /tmp/dir1/dir2
crear un árbol de directorios.

## rm -f file1
borrar el fichero llamado ‘file1’.

## rmdir dir1
borrar la carpeta llamada ‘dir1’.

## rm -rf dir1
eliminar una carpeta llamada ‘dir1’ con su contenido de forma recursiva. (Si lo borro recursivo estoy diciendo que es con su contenido).

## rm -rf dir1 dir2
borrar dos carpetas (directorios) con su contenido de forma recursiva.

## mv dir1 new_dir
renombrar o mover un fichero o carpeta (directorio).

## cp file1
copiar un fichero.

## cp file1 file2
copiar dos ficheros al unísono.

## cp dir /* .
copiar todos los ficheros de un directorio dentro del directorio de trabajo actual.

## cp -a /tmp/dir1 .
copiar un directorio dentro del directorio actual de trabajo.

## cp -a dir1
copiar un directorio.

## cp -a dir1 dir2
copiar dos directorio al unísono.

## ln -s file1 lnk1
crear un enlace simbólico al fichero o directorio.

## ln file1 lnk1
crear un enlace físico al fichero o directorio.

## touch -t 0712250000 file1 
modificar el tiempo real (tiempo de creación) de un fichero o directorio.

## file file1
salida (volcado en pantalla) del tipo mime de un fichero texto.

## iconv -l
listas de cifrados conocidos.

# Encontrar Archivos.

## find / -name file1
buscar fichero y directorio a partir de la raíz del sistema.

## find / -user user1
buscar ficheros y directorios pertenecientes al usuario ‘user1’.

## find /home/user1 -name *.bin
buscar ficheros con extensión ‘. bin’ dentro del directorio ‘/ home/user1’.

## find /usr/bin -type f -atime +100
buscar ficheros binarios no usados en los últimos 100 días.

## find /usr/bin -type f -mtime -10
buscar ficheros creados o cambiados dentro de los últimos 10 días.

## find / -name *.rpm -exec chmod 755 ‘{}’ ;
buscar ficheros con extensión ‘.rpm’ y modificar permisos.


# Comandos Docker

## build	
Construir una imagen a partir de un Dockerfile

## history	
Mostrar el historial de una imagen

## import	
Importar el contenido de una tarball para crear una imagen del sistema de archivos

## inspect
Mostrar información detallada sobre una o más imágenes

## load
Cargar una imagen de un archivo tar o STDIN

## ls	
Listar imágenes

## prune	
Eliminar imágenes no utilizadas

## pull	
Extraer una imagen o un repositorio de un registro

## push	
Empujar una imagen o un repositorio a un registro

## rm	
Eliminar una o más imágenes

## save	
Guardar una o más imágenes en un archivo tar 

## tag	
Cree una etiqueta TARGET_IMAGE que haga referencia a SOURCE_IMAGE
