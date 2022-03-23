# Introducción a los Comandos de Linux

[![CST Logo](./figures/logo.png)](https://cloud-systems-technology.com.mx)

---

## Accesos de Teclado

Teclas | Descripción
--- | ---
`[CTRL + ALT + F<n>]` | Abre la `<n>` terminal virtual (`TTY<n>`). **Nota:** `TTY7` es comunmente la terminal gráfica.
`[CTRL + ALT + T]` | Abre una terminal emulada en el modo gráfico.
`[CTRL + L]` | Limpia la terminal (recorre la vista).

## Comandos de Linux

Comando | Descripción
--- | ---
`pwd` | Muestra el directorio actual de trabajo (`/home/<username>`)
`cd <path>` | Cambia el directorio actual por el especificado o el del usuario
`ls` | Muestra los archivos del directorio actual
`ls -l` | Muestra la lista más descriptiva con permisos y otros datos
`man <command>` | Muestra la documentación de un comando
`info <command>` | Muestra información de un comando
`apt update` | Actualiza la lista de fuentes
`apt upgrade` | Aplica las actualizaciones pendientes
`apt list --installed` | Muestra los paquetes instalados
`apt list --upgradable` | Muestra los paquetes actualizables
`apt show <package>` | Muestra la información de un paquete
`apt install <package>` | Instala un paquete
`nano <path>/<file>` | Abre un editor sencillo de texto (`[CTRL+O] Guardar [CTRL+X] Salir`)
`useradd -m -d <home>/<username> -s /bin/bash <username>` | Crea un nuevo usuario del sistema
`id` | Muestra la información de usuario actual
`id <username>` | Muestra la información del usuario solicitado
`whoami` | Muestra el nombre del usuario actual
`passwd <username>` | Establece la contraseña del usuario
`passwd -Sa` | Muestra el estado de las contraseñas para todos los usuarios
`passwd -S <username>` | Muestra el estado de las contraseñas para todos los usuarios
`su - <username>` | Inicia sesión con el usuario solicitado
`exit` | Cierra la sesión (en la terminal) del usuario
`usermod -a -G sudo <username>` | Convierte a un usuario en administrador (lo agrega al grupo `sudo`)
`usermod -G <username> <username>` | Le quita los grupos adicionales al usuario (reestrablece al usuario como un usuario tradicional/estándar)
`passwd -e <username>` | Obligar al cambio de contraseña (expiramos la contraseña actual)
`usermod -L <username>` | Bloquea la cuenta de usuario solicitada
`usermod -U <username>` | Desbloquea la cuenta de usuario solicitada
`passwd -l <username>` | Bloquea la contraseña del usuario solicitado
`passwd -u <username>` | Desbloquea la contraseña del usuario solicitado
`usermod -e 0 <username>` | Expira la cuenta de usuario solicitada (la deja inactiva de forma efectiva)
`usermod -e YYYY-MM-DD <username>` | Programa la expiración de la cuenta
`sudo usermod -e 99999 <username>` | Quita la fecha de expiración de la cuenta solicitada
`who -u` | Muestra la lista de usuarios activos
`kill <pid>` | Mata un proceso específico
`chfn <username>` | Cambia la información del usuario solicitado
`finger` | Muestra la información de los usuarios
`finger -s <username>` | Muestra la información del usuario solicitado
`more <file>` | Muestra el contenido del archivo por páginas
`cat <file 1> ... <file n>` | Concatena el o los archivos en la salida estándar (muestra)
`less <file>` | Muestra el contenido de un archivo por páginas
`lynx <url>` | Abre un navegar web en modo texto para la url solicitada
`mkdir <dir>` | Crea una nueva carpeta con el nombre especificado
`mount <device> <path>` | Montar un dispositivo en la carpeta especificada
`mount -l` | Ver los dispositivos montado
`umount <device>` | Desmonta un dispositivo de su carpeta montada


## Rutas importantes de Linux (Sistema de archivos)

Ruta | Descripción
--- | ---
`/` | Raíz del sistema de archivos (el directorio principal, en Windows equivaldría a `C:\`)
`/bin` | Se encuentran los archivos ejecutables del sistema
`/sbin` | Se encuentras los archivos ejecutables del usuario
`/dev` | Se encuentran los dispositivos físicos y lógicos en forma de archivos especiales
`/boot` | La carpeta de montaje
`/root` | La carpeta del usuario `root` (el administrador)
`/home` | La carpeta que contiene las carpetas de los usuarios
`/lib` | La carpeta de las librerías del sistema
`/etc` | La carpeta de archvios y configuraciones usada por aplicaciones instaladas
`/usr` | La carpeta de archivos generados por las instalaciones para el usuario
`/opt` | Similar a `/etc` pero para programas compartidos
`/var` | La carpeta de configuraciones adicionales de los programas
`/tmp` | La carpeta de archivos temporales (caché)
`/media` | Una carpeta diseñada para montar unidades
`/sys` | Una carpeta con cosas del sistema
`/usr/share/doc/<command>` | Contiene la documentación adicional del comando
`~` | Se refiere a la carpeta del usuario
`~<username>` | Se refiere a la carpeta del usuario especificado

## Dispositivos y Montado

Cuándo linux detecta un nuevo dispositivo creará un archivo lógico dentro de `/dev`, por ejemplo, si conectamos un nuevo disco duro o una memoria usb, generalmente saldrá registrada como `/sd<X>` (ejemplo `/dev/sda`, `/dev/sdb`, `/dev/sdc`, ...).

Los dispositivos de almacenamiento contienen una tabla de particiones, la cuál permite informarle al sistema sobre los sectores utilizables para el almacenamiento. Generalmente las memorias USB contienen una sola partición y también los discos duros. Sin embargo, hay discos particionados en múltiples sectores, cada partición reservando sus propios sectores, lo que hace que el disco funcione como si fueran dos o más discos duros.

Cuándo un medio tiene particiones estas serán registradas como `/dev/sdb<X><N>` (ejemplo `/dev/sdb1`, `/dev/sdb2`, ...).

Los comandos más útiles para trabar con medios de almacenamiento son `lsblk`, `fdisk`, `mkfs.<...>`, `mount` y `umount`.