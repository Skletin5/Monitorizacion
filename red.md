# Trafico de Red
En nuestro equipos circulan diariamente grandes cantidades de información, accediendo a este y saliendo del mismo a traves de la red.
Es importane vijilar dicho trafico para detectar problemas o incluso ataques a nuestro servidor.

## TCPDUMP
Esta herramienta analiza el tráfico que circula por la red. Primero debemos instalarlo:

`$ sudo apt install tcpdump`

Tras su instalación, lo utilizamos de la siguiente manera:

`$ tcpdump [Opciones] [Filtros]`

Ejemplo:  
![tcpdump](/img/red/tcpdump.PNG)
Las opciones que podemos agregar son:  
-`-c [cantidad]`: Analiza la cantidad de veces indicada.  
-`-D` Muestra una lista de todas las interfaces disponibles por numeros.  
-`-i [interfaz]`: Se especifica un interfaz a capturar.  
-`-s [cantidad]`: Captura la cantidad de bytes por paquete.  

Podemos aplicar los siguientes filtros:
-`-dst`: solo se analizan paquetes cuyo destino coincide con el valor establecido. Este valor puede ser host, net, port o portrange.  
-`-host`: este filtro se ocupa de que solo se tengan en cuenta los paquetes que tienen una dirección IP específica como origen o destino, o en su lugar, un nombre de host específico.  
-`-net`: este filtro solo considera los paquetes que tienen una dirección IP dentro de un rango de red específico como origen o destino.  
-`-port`: con este filtro se especifica un puerto específico entre 0 y 65535, que se analizará de forma exclusiva.  
-`-portrange`: este filtro contiene un rango de puertos entre 0 y 65535 que se analizará de forma exclusiva.  
-`-proto`: este filtro solo considera los paquetes con un protocolo de red específico. El filtro puede tener los siguientes valores: arp, decnet, ether, fddi, ip, ip6, rarp, tcp, udp o wlan.  
-`-src`: solo se analizan los paquetes cuyo origen coincide con un valor establecido. Este valor puede ser host, net, port o portrange.  

## TCPTRACK
Nos muestra las conexiones establecidas, su origen, destino, estado, el tiempo de idle y la velocidad de transferencia. Deberemos instalarlo primero:

`$ sudo apt install tcptrack`

Podemos ejecutarlo así:

`$ tcptrack`

Ejemplo:
![tcptrack](/img/red/tcptrack.PNG)  

Una opción que podemos usar es `-i [nombre interfaz]` para escanear el trafico de una interfaz especifica.

## IPTRAF
Intercepta paquetes en la red y muestra información sobre el tráfico. Se instala así:

`$ sudo apt install iptraf-ng`

para ejecutarlo escribimos:

`$ sudo iptraf`

Ejemplo:
![iptraf](/img/red/iptraf.PNG)

Nos despliega un menu con el que podemos trabajar.
