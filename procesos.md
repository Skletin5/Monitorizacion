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
-  `-x`: Muestra los procesos del usuario ejecutor.  

## TOP
Este comando nos permite ver los procesos en ejecución en tiempo real y detalles sobre el mismo como el consumo de cpu o el nombre del proceso.

`$ top`

Ejemplo:
![top solo](/img/procesos/top_solo.PNG)

Durante su ejecución podemos interactuar con distintas teclas para modificar como nos muestra la información.  
- `C`: Alterna entre mostrar el nombre del proceso y el comando completo.  
- `T`: Ordena por tiempo de ejecución.  
- `M`: Ordena por uso de memoria.  
- `F`: Lleva a una ventana que permite elegir que información deseamos que nos muestre la tabla.  
- `R`: Te permite reiniciar un proceso.  
- `K`: Te permite matar un proceso.  

## HTOP
Similar a top, pero con una interfaz más visual y funciones adicionales, como la capacidad de desplazarse y filtrar procesos de manera más intuitiva.

`$ htop`

Ejemplo:
![htop](/img/procesos/htop.PNG)

Justo debajo vemos todas las opciones que nos da esta herramnienta, pero existen unos pocos atajos para ordenar la información:  
-`M`: Ordena por uso de memoria.  
-`P`: Ordena por uso de procesador.  
-`T`: Ordena por tiempo de ejecución.  
-`F`: Permite marcar un proceso para facilitar sus seguimiento.  
-`K`: Despliega una lista de señales que mandarle a los procesos, como por ejemplo "kill".  

## ATOP
Como todos los anteriores, pero ademas registra e informa de toda la actividad de todos los procesos del servidor.

`$ atop`

Ejemplo:
![atop](/img/procesos/htop.PNG)

Podemos ordenar la informacion con estar teclas:  
-`A`: Ordena por recurso del sistema mas utilizado.  
-`C`: Ordena por consumo de cpu.  
-`D`: Ordena por accesos al SSD o disco duro.  
-`M`: Ordena por uso de memoria.  
-`N`: Ordena por ancho de banda de red utilizado.  

Pero tambien nos permite almacenar los datos en un fichero para vovler a consultarlos con otro comando de atop, ya que los almacena en formatobinario.  
`$ atop -w [ruta del archivo]`

luego podemos volver a consultarlo con el siguiente comando:  
`$ atop -r [ruta del archivo]`
