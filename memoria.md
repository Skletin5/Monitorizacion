# Memoria
Para que nuestro servidor trabaje correctamente es indispensale que disponga de memoria suficiente para sus procesos y espacio de almacenamiento. Por lo que la monitorización de los mismos es crucial para asegurar el correcto funcionamiento del mismo.

Existen varios comando que nos permite llevar acabo dichas tareas:

## Free
Este comando proporciona toda la información sobre la RAM, cuanta RAM se está utilizando, cuenta está disponible, etc.

`$ free [Opciones]`

Ejemplo:  
![free](/img/memoria/free.PNG)

Podemos agregar opciones como:  
-`-h`: Facilita la lectura mostrando los datos en Mb, Gb...  
-`-s [tiempo en segundos]`: Se ejecuta durante un tiempo designado.  
-`-c[numero]`: muestra el numero de salidas indicadas junta a la opción (debe estar junto a la opción sin espacio)

## DF
Muestra el espacio utilizado y disponible en los sistemas de archivos montados.

`$ db [Opciones]`

Ejemplo:
![df](/img/memoria/df.PNG)

Podemos agregar opciones como:  
-`-h`: Igual que en free, nos muestra los datos en Mb y Gb.  
-`-i`: Nos muestran sistemas de ficheros con 0 bytes.  
-`-a`: Muestra todos los ficheros.

## DU
 Muestra el espacio ocupado por un fichero o directorio.

`$ du [opciones]`

Ejemplo:
![du](/img/memoria/df.PNG)

Podemos agregar opciones como:  
-`-h`: Muestra la informacion en Mb o Gb.  
-`-s`: MUestra la informacion en la carpeta actual y no subcarpetas.

## IOSTAT
Se utiliza para rastrear los problemas de rendimiento de los dispositivos de
almacenamiento.

`$ iostat [Opciones]`

Ejemplo:
![iostat](/img/memoria/iostat.PNG)

Podemos agregar opciones como:
-`-c`: Muestra información sobre la CPU.
-`-d`: Muestra informacion sobre los dispositivos de E/S.
-`-x`: Muestra información mas detallada.
-`-k`: Muestra los datos en Kb.
-`-m`: Muestra la informacion en Mb.
