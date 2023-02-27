# Redes Cableadas
---


Utiliza un cable especial que se divide en varios pares de cobre. Este tipo de cable recibe el nombre de cableado estructurado (STP, apantallado para evitar interferencias electromagnéticas y UTP, sin apantallar, más común). Siguen distintas normas (con un código de colores para cada cable). Al final de estos cables se ponen conectores para unir a equipos informáticos (“capuchones” de plástico). Los utilizados para cableado de red son los denominados RJ-45 (los que se usan para conectar el router a la línea de teléfono son parecidos pero más pequeños, RJ-11, no confundir).

<figure markdown>
  ![Imatge 1](../../img/imatge1.png){ width="500" }
  <!-- <figcaption>Image caption</figcaption> -->
</figure> 

Vemos una ilustración para ver la correspondencia de colores que deben cumplirse para realizar cableado estructurado:

<figure markdown>
  ![Imatge 2](../../img/imatge2.png){ width="500" }
  <!-- <figcaption>Image caption</figcaption> -->
</figure> 




Hoy en día está en desuso el cableado cruzado, y se usa normalmente sólo el paralelo. El cableado paralelo sin proteger (UTP) puede conseguir una velocidad de 100 Mbits/s máximo (Mb/s). Si falla algún par de cables, se reduce la velocidad a 10 Mb/s. Si fallan más, no conectaría. Con el STP y categorías superiores de cable, se pueden conseguir velocidades mayores, pero se atenúan con la longitud de cable.

!!!success "Ventajas de la utilización de redes cableadas"
    Rapidez dentro de tu red. Imposiblidad de intrusión externa.


!!!failure "Desventajas de la utilización de redes cableadas"  
    Necesita cables que en ocasiones no se pueden instalar fácilmente y atravesar paredes, etc… (“tirar cableado”).. También pueden deteriorarse (tirones en el capuchón/conector o cortes en cable).



## Tarjeta de Red (Cableada)
   
Hoy en día el protocolo que se usa es el Ethernet, que se usa en todos los PC actuales (excepto en algún netbook, que sólo lleve wifi). Antiguamente había más, como el Token Ring de IBM que está desapareciendo.

<figure markdown>
  ![Imatge 3](../../img/tarjetared.png){ width="300" }
  <figcaption>Tarjeta de red</figcaption>
</figure> 


 
   
## Hardware de Interconexión (Cableada)
   
Para la conexión de distintos equipos y la distribución de paquetes más eficiente, se usan switch cableados, los hay de muchos tamaños y precios. El router típico doméstico trae incorporado un switch también de 4 puertos. También hay **hubs**, más baratos aunque pueden saturar la red, dado que mandan todos los datos a todos los ordenadores. También son más inseguros por la misma razón. Hoy en día están en desuso. Otra alternativa es la tecnología **PLC** (*power line communication*), que ofrece conexión a Internet a través de la red eléctrica. Esta tecnología permite utilizar el cableado de la red eléctrica ya existente para transmitir audio, datos y televisión. La velocidad de una red local que utilice PLC puede llegar hasta los 400 Mbits/segundo. En España no ha tenido mucho éxito debido a problemas técnicos, aunque se espera que en un futuro cercano se extienda su uso, al menos en el ámbito doméstico.


<figure markdown>
  ![Imatge 4](../../img/cableado.png){ width="400" }
  <figcaption>Rack de comunicaciones</figcaption>
</figure> 
