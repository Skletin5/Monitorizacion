En nuestros sistemas y servidores dispondremos de innumerables aplicaciones y programas en constante funcionamiento, y el fallo de uno de ellos
podria interrumpir su servicio. Por lo que es muy importante mantenerlos a raya y preveer posibles fallos.

A continuacion veremos algunos comandos que nos posibilitan llevar a cabo esta tarea.

## PS
Este comando te muestra una lista con todos los procesos que se estén ejecutando en el sistema en ese momento.

`$ ps [Opciones]`

Ejemplo: 
![ps solo](/img/procesos/ps_solo.PNG)
Existen distintas opciones que nos permiten trabajar con este comando:
- `-A`: Muestra todos los procesos que se esten ejecutando en el sistema y de todos los usuarios.
- `-a`: Muestra solo los procesos asociados a la terminal desde la que se ejecuta.
- `-C [procesos]`: Muestra solo los procesos nombrados.
- `-d`: Muestra los procesos sin los nombres de usuario asignados.
- `-e`: Igual que -A.
- `-f`: Muestra todos los procesos en mayor detalle.
- `-r`: Muestra solo los procesos en ejecucion en el momento de ejecución.
-  `-T`: Igual que -a.
-  `-x`: Muestra los procesos del usuario ejecutor

## TOP
