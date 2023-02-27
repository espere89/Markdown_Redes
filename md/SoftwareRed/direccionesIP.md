# Direcciones IP
---

Las direcciones IP son conjuntos de números que identifican a un equipo dentro de una red. Cada número puede estar en el intervalo [0..255], o sea, 256 números. Se puede simbolizar cada equipo con un número en binario de 8 bits. Se reservan el 0, que significa “la propia red” y el 255 que simboliza “para todos los equipos” (llamado dirección de broadcast). 
    
Inicialmente, el protocolo se diseñó para unos 255 ordenadores, pero se sobredimensionó para que pudiera dar servicio a muchos más ordenadores en un futuro. Por eso no les bastaba con un solo número de 8 bits.  
    
Al principio, se hizo la norma IPv4 con 4 números de 8 bits (xx.xx.xx.xx donde xx es un número de los anteriores). con esto se llegaba a más de 4 mil millones de equipos. Sin embargo, con el estado actual de conexión de equipos, se hizo necesario ampliar estos números, dado que podía darse un agotamiento de direcciones en el mundo. por eso se creó el IPv6, con seis números. 
    
En un principio, esto soluciona el problema hasta que haya 240 mil millones de equipos conectados (la población mundial no supera los ocho mil millones en este momento, 7400 en diciembre de 2016). Para este tema, estudiaremos el caso de IPv4 (IPv6 es prácticamente igual).


### Tipos de dirección IP 
    
Los categorizaremos en una tabla:

|  | Fija | Dinámica (DHCP) |
| :---: | :--- | :--- |
| Local (Privada) | IP local típica en un entorno controlado como empresas, negocios. | IP local típica en una instalación doméstica. |
| WAN (Pública) | IP asignada por el ISP a una compañía que requiera tener siempre la misma IP (por ejemplo para tener una página web o servidor). Se puede tener en casa, pero se paga por ello. | IP que asigna un ISP a un usuario normal en la mayoría de los casos. |

En cuanto alcance y visibilidad

- **IP local:** es un número que identifica el equipo dentro de tu propia red. Se podría repetir en otras redes (o sea, que en el Instituto un portátil podría tener el número IP 192.168.0.124 y en casa tener el mismo igual o cambiado en alguno de los números).
- **IP Pública:** dirección única dentro de la red. Es la dirección dentro de Internet, y para la gente que observa desde fuera de tu red, todos los ordenadores de una red tienen la misma IP Pública.
    
En cuanto a comportamiento en el tiempo 
    
- **IP Fija:**  La determinamos nosotros en el propio equipo. El equipo encargado de la Capa de Transmisión (suele ser el router) lo aceptará si está dentro de los números admisibles (depende de la máscara de red). Se utiliza en redes donde prima el control. Donde sí es necesario y deseable que haya direcciones fijas es en los elementos de red (router siempre, puntos de acceso, y switch si son gestionables). 

 - **IP Dinámica (DHCP):** El router determina cada vez que te conectas qué número asignarte dentro de un rango de disponibles (pool DHCP). Se mantiene este número durante un tiempo, para evitar perder tiempo en reconectar aparatos que se van unas horas (móviles, por ejemplo) y luego vuelven en menos de un par de días. 

    
### Otras direcciones IP importantes

- **DNS:** son servidores de Internet que convierten una dirección en letras [www.google.es](www.google.es) en su dirección IP pública. Es posible que estos servidores tengan un problema y no podamos conectar a páginas de Internet sin que sea problema de nuestra línea. Para evitar este problema, podemos configurar de forma manual las DNS que usaremos, aunque las que nos asigna el ISP suelen ser más rápidas en darnos servicio. Para eso sería conveniente tener una lista de DNS de otros operadores distintos al nuestro y otras de nuestro propio operador a mano (en el momento de la avería no podemos consultarlas en internet).

- **Puerta de enlace:** dirección del router o dispositivo que manda la información a Internet. En tu casa, suele ser del tipo 192.168.0.1, o acabados en 1.1, 2.1, etc… aunque se podría cambiar al número que deseemos. En general, se deja este formato (192.168.X.X) o se usan los 10.X.X.X si se quiere hacer redes más grandes. También es la dirección del dispositivo de red del ISP que recibe tu conexión, será interesante tener este dato apuntado ante una caída en Internet para descartar fallos. 

## Dirección Física

- **MAC:** Dirección física que tiene una tarjeta de red (en un principio es única). Es en código hexadecimal con este formato: 00-11-85-17-2F-33 Los distintos fabricantes de tarjetas de red se reservan numeración. Esta numeración puede consultarse en Internet (mac vendor list), de forma que si ponermos una MAC nos diga el fabricante (no dice el modelo ni la marca del ordenador, sólo el fabricante de la tarjeta de red).