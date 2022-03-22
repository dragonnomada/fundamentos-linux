# CST - Fundamentos de Linux

[![CST Logo](./figures/logo.png)](https://cloud-systems-technology.com.mx)

---

## Descripción general

Orientado para aquellos que van a acercarse por primera vez a Linux. Se capacita al usuario para que
aprenda a instalarlo en su equipo, comience a trabajar en el entorno gráfico con las aplicaciones
instaladas y en la terminal con el shell bash. También se tratan los temas de manejo de archivos y
personalización del entorno de trabajo.

## Objetivos

El curso introduce al estudiante para que entienda que es Linux, aprenda a instalarlo y a trabajar en el
entorno gráfico y en el shell con los archivos y aplicaciones del sistema.

## Contenido

> Capítulo 1 Introducción 

- A. Historia de Unix.  
- B. GNU.  
    1. FSF.  
    2. CopyLeft y GPL.  
- C. Linux.  
    1. Características.  
    2. Distribuciones. 
- D. ¿Qué distribución elegir?.  
    1. Las distribuciones para el "gran público".  
    2. Las distribuciones "móviles".  
    3. Las distribuciones "profesionales".  
    4. Las distribuciones "especializadas".   
- E. Convenciones tipográficas.  
    1. Estilos de letra.  
    2. Teclado. 

> Capítulo 2 Inicio de sesión y primeros comandos  

- A. Introducción.  
- B. Consolas y terminales Linux.  
    1. Consolas virtuales.  
    2. Emuladores de terminales.  
    3. Terminales remotos.  
- C. Inicio de sesión, autenticación.  
- D. Símbolo del sistema del shell (prompt). 
- E. Sintaxis de los comandos.  
- F. Uso del ratón.  
- G. Atajos de teclado.  
    1. En modo texto.  
    2. En modo gráfico.  
- H. Primeros comandos.  
    1. Identidad de los usuarios: who, whoami, finger.  
    2. Cambio de contraseña: passwd.  
    3. Conteo: wc.  
    4. Visualización: clear, echo.  
    5. Tiempo: date, cal.  
- I. Cerrar sesión.

> Capítulo 3 Documentación 

- A. Introducción.  
- B. Manual.  
    1. Secciones. 
    2. Comando man. 
    3. /etc/man.config. 
- C. Documentación Info.  
    1. Comando info.  
- D. Opción --help de los comandos en Linux.  
- E. Documentación HOWTO.  
- F. /usr/share/doc.  
- G. Internet.  
    1. Sitios.  
    2. Grupos de discusión. 

> Capítulo 4 El árbol de Linux 

- A. El árbol de Linux.  
- B. Directorios principales.  
    1. /bin, /sbin, /lib.  
    2. /boot.  
    3. /dev.  
    4. /home.  
    5. /root. 
    6. /tmp. 
    7. /lost+found. 
    8. /mnt.  
    9. /proc.  
    10. /sys.  
    11. /usr.  
    12. /var.  
    13. /etc. 
- C. Montar y acceder a los medios extraibles.  
    1. Comando mount.  
    2. Comando umount.  
    3. Caja de herramientas mtools. 

> Capítulo 5 Manipulación de archivos 

- A. Introducción.  
- B. Nombres de archivos y de directorios.  
- C. Tipos de archivos.  
- D. Rutas.  
    1. Rutas absolutas.  
    2. Rutas relativas.  
    3. Rutas personales.  
- E. Exploración del árbol.  
    1. pwd.  
    2. cd.  
    3. ls.  
    4. file.  
    5. stat.  
- G. Archivos  
    1. touch.  
    2. cp.  
    3. rm.  
    4. mv.  
- H. Organización física de los archivos en Linux.  
    1. Inodos y bloques de datos.  
- I. Administradores de archivos.  
    1. Midnight Commander.  
    2. Konqueror, Nautilus. 

- J. Consultar archivos.  
    1. cat.  
    2. more, less.  
    3. od, strings. 

> Capítulo 6 Edición de archivos de texto – Vi 

- A. Introducción.  
- B. Presentación de Vi.  
    1. Inicio de Vi.  
    2. Modos de funcionamiento.  
    3. Comandos de desplazamiento.  
    4. Comandos de inserción.  
    5. Comandos de edición y de corrección.  
    6. Comandos globales.  
    7. Archivo de configuración personal.  
    8. Otros comandos útiles.  
- C. Otras herramientas de edición  
    1. Otros editores de texto.  
    2. Editores hexadecimales. 

> Capítulo 7 Permisos de acceso a los archivos 

- A. Conceptos de cuentas de usuario y de grupos.  
    1. Jerarquía de usuarios.  
    2. Comandos útiles.  
- B. Permisos de Unix.  
    1. Permisos estándar.  
    2. SUID, SGID y Sticky Bit. 
- C. Administrar permisos.  
    1. chgrp.  
    2. chmod. 
    3. umask.  
    4. Administradores de archivos. 

> Capítulo 8 Administración de procesos 

- A. Introducción.  
- B. Árbol de procesos y PID.  
- C. Visualización de los procesos.  
    1. ps.  
    2. top.  
    3. pstree.  
- D. Señales y comando kill.  
- E. Administradores de procesos gráficos.  
- F. Trabajo con procesos.  
    1. Iniciar un proceso.  
    2. Detener un proceso.  
    3. Controlar los procesos iniciados desde la línea de comandos. 

> Capítulo 9 Shell Bash 

- A. Introducción.  
- B. Generalidades y definiciones.  
- C. Variables.  
    1. Trabajo con variables.  
    2. Variables de entorno.  
- D. Caracteres genéricos.  
- E. Caracteres de cita.  
- F. Redirecciones.  
    1. Descriptores de archivos.  
    2. Redirección de la entrada estándar.  
    3. Redirección de la salida estándar.  
    4. Redirección del error estándar. 
    5. Redirecciones combinadas.  
    6. Ejemplos de redirecciones.  
    7. Los tubos.  
- G. Alias.  
- H. Ejecución de comandos.  
    1. type, whereis.  
- I. Sustitución de comandos.  
- J. Opciones del shell Bash.

---

## Capítulo 1 Introducción 

    A. Historia de Unix.  
    B. GNU.  
        1. FSF.  
        2. CopyLeft y GPL.  
    C. Linux.  
        1. Características.  
        2. Distribuciones. 
    D. ¿Qué distribución elegir?.  
        1. Las distribuciones para el "gran público".  
        2. Las distribuciones "móviles".  
        3. Las distribuciones "profesionales".  
        4. Las distribuciones "especializadas".   
    E. Convenciones tipográficas.  
        1. Estilos de letra.  
        2. Teclado. 

### Ejercicio 1.1

    Responde las siguientes preguntas:

    ¿Qué es la FSF?

    ¿Qué garantiza el Copyleft?

    ¿Quién promovió el uso de software libre y en qué año?

    ¿Qué es el GPL?

    ¿Quién diseño Linux y qué diferencia tiene con UNIX?

### Ejercicio 1.2

    Menciona tres características de linux

    Menciona tres distribuciones de linux y sus diferencias

### Ejercicio 1.3

    ¿Cuál es la ruta usada para almacenar los estilos de fuentes compartidos y locales al usuario?

    ¿Con qué programa podemos editar un archivo de estilos de fuentes?

### Ejercicio 1.4

    ¿Cuáles son las teclas para cambiar a otra terminal del sistema?

    ¿Cuáles son las teclas para suspender y reanudar un programa?

    ¿Cuáles son las teclas para buscar un comando ejecutado?

## Capítulo 2 Inicio de sesión y primeros comandos  

    A. Introducción.  
    B. Consolas y terminales Linux.  
        1. Consolas virtuales.  
        2. Emuladores de terminales.  
        3. Terminales remotos.  
    C. Inicio de sesión, autenticación.  
    D. Símbolo del sistema del shell (prompt). 
    E. Sintaxis de los comandos.  
    F. Uso del ratón.  
    G. Atajos de teclado.  
        1. En modo texto.  
        2. En modo gráfico.  
    H. Primeros comandos.  
        1. Identidad de los usuarios: who, whoami, finger.  
        2. Cambio de contraseña: passwd.  
        3. Conteo: wc.  
        4. Visualización: clear, echo.  
        5. Tiempo: date, cal.  
    I. Cerrar sesión.

### Ejercicio 2.1

    # Crear un usuario y su carpeta de usuario

    1. Inspecciona el comando `useradd` con `man`

        [$] man useradd

    2. Crea un usuario nuevo con `useradd` y establece su carpeta de usuario y la terminal `/bin/bash`

        [#] useradd -m /home/<username> -s /bin/bash <username>

    3. Inspecciona el comando `id` con `man`

        [$] man id

    4. Obtén la información del usuario creado con `id`

        [$] id <username>

    5. Inspecciona el comando `passwd` con `man`

        [$] man passwd

    6. Crea una contraseña para el usuario nuevo con `passwd`

        [#] passwd <username>

    7. Inspecciona el comando `ls` con `man`

        [$] man ls

    8. Obtén la información de la carpeta `/home` con `ls`

        [$] ls -la /home

    9. Inspecciona el comando `cd` con `man`

        [$] man cd

    10. Navaga a la carpeta del usuario creado con `cd`

        [$] cd ~<username>

### Ejercicio 2.2

    # Iniciar sesión con el usuario creado

    1. Inicia sesión con el usuario creado

        [#] su - <username>

    2. Inspecciona el comando `pwd` con `man`

        [$] man pwd

    3. Obtén la información del directorio actual con `pwd`

        [$] pwd

    4. Inspecciona el comando `whoami` con `man`

        [$] man whoami

    5. Obtén la información del usuario actual con `whoami`

        [$] whoami

    6. Cierra la sesión del usuario creado con `exit`

        [$] exit

    7. Vuelve a obtener la información del usuario actual con `whoami`

### Ejercicio 2.3

    # Iniciar sesión con el usuario creado en `tty3`

    1. Pulsa las teclas `ctl+alt+f3`

        [CTRL + ALT + F3]

    2. Inicia sesión con el usuario creado

        Login: <username>
        Password: <<****>>

    3. Ejecuta el comando `id`

        [$] id

    4. Cierra sesión con `exit`

### Ejercicio 2.4

    # Bloquar un usuario

    1. Inspecciona el comando `usermod` con `man`

        [$] man usermod

    2. Bloquea el usuario creado con `usermod`

        [#] usermod -L <username>

    3. Intenta iniciar sesión con el usuario

        [#] su - <username>

    4. Desbloquea el usuario creado con `usermod`

        [#] usermod -U <username>

    5. Intenta iniciar sesión con el usuario

        [#] su - <username>

    6. Bloquea la contraseña del usuario creado con `passwd`

        [#] passwd -l <username>

    7. Intenta iniciar sesión con el usuario creado

        [#] su - <username>

    8. Desbloquea la contraseña del usuario creado con `passwd`

        [#] passwd -l <username>

    9. Intenta iniciar sesión con el usuario creado

        [#] su - <username>

    10. Expira la fecha del usuario creado con `passwd`

        [#] passwd -e <username>

### Ejercicio 2.5

    # Iniciar sesión mediante GNOME

    1. Inspecciona el comando `who` con `man`

        [$] man who

    2. Obtén la sesión actual del usuario con `who`

        [$] who -u

    3. Cierra la sesión actual con `kill`

        [$] kill <pid>

    4. Inicia sesión con el nuevo usuario creado

        User: <username>
        Password: <<****>>

### Ejercicio 2.6

    # Información de usuarios

    1. Inspecciona el comando `chfn` con `man`

        [$] man chfn

    2. Cambia la información del usuario creado

        [#] chfn <username>

    3. Instala `finger` con `apt`

        [#] apt install finger

    4. Inspecciona el comando `finger` con `man`

        [$] man finger

    5. Obtén la información de los usuarios con `finger`

        [$] finger

    6. Obtén la información del usuario creado con `finger`

        [$] finger <username>

## Capítulo 3 Documentación 

    A. Introducción.  
    B. Manual.  
        1. Secciones. 
        2. Comando man. 
        3. /etc/man.config. 
    C. Documentación Info.  
        1. Comando info.  
    D. Opción --help de los comandos en Linux.  
    E. Documentación HOWTO.  
    F. /usr/share/doc.  
    G. Internet.  
        1. Sitios.  
        2. Grupos de discusión. 

### Ejercicio 3.1

    # Navegar páginas desde la terminal

    1. Instalar `lynx`

        [#] apt install lynx

    2. Abrir una página

        [$] lynx google.com

    3. Busca la página `man page` en `google`

        >> Ubica ________ y escribe "man page"

## Capítulo 4 El árbol de Linux 

    A. El árbol de Linux.  
    B. Directorios principales.  
        1. /bin, /sbin, /lib.  
        2. /boot.  
        3. /dev.  
        4. /home.  
        5. /root. 
        6. /tmp. 
        7. /lost+found. 
        8. /mnt.  
        9. /proc.  
        10. /sys.  
        11. /usr.  
        12. /var.  
        13. /etc. 
    C. Montar y acceder a los medios extraibles.  
        1. Comando mount.  
        2. Comando umount.  
        3. Caja de herramientas mtools. 

### Ejercicio 4.1

    Describe las siguientes carpetas del sistema

    /bin
    /boot
    /dev
    /etc
    /home
    /lib
    /media
    /root
    /sbin
    /tmp
    /usr
    /var



---

[![Alan Badillo Salas](https://avatars.githubusercontent.com/u/79223578?s=40&v=4 "Alan Badillo Salas")](https://github.com/dragonnomada) Instructor [Alan Badillo Salas](https://github.com/dragonnomada)

Estudié **Matemáticas Aplicadas** en la Universidad Autónoma Metropolitana, posteriormente realicé una Maestría en **Inteligencia Artificial** en el Instituto Politécnico Nacional.

He impartido cursos de Programación Avanzada en múltiples lenguajes de programación, incluyendo *C/C++, C#, Java, Python, Javascript* y plataformas como *Android, IOS, Xamarin, React, Vue, Angular, Node, Express*. Ciencia de Datos en *Minería de Datos, Visualización de Datos, Aprendizaje Automático y Aprendizaje Profundo*. También sobre *Sistemas de administración basados en Linux, Apache, Nignx* y *Bases de Datos SQL y NoSQL* como MySQL, SQL Server y Mongo. Desde hace 7 años en varios instituciones incluyendo el *IPN-CIC, CST, KMMX, The Inventor's House, Auribox*. Para diversos clientes incluyendo al *INEGI, CFE, PGJ, SEMAR, Universidades, Oracle, Intel y Telmex*.

---