# Seguridad en redes Wifi
---

<figure markdown>
  ![Imatge 8](../../img/security.png){ width="300" }
</figure>

La información se manda codificada según la opción de seguridad elegida. Podremos ir incrementando la seguridad según nuestras necesidades. De menos a más seguras:

- **Abierta**: Nada seguras. Cualquier dispositivo puede unirse. Se recomienda no utilizar redes abiertas (otros usuarios podrían poner en riesgo nuestro equipo) o hacerlo con mucha precaución (sin introducir datos personales mientras usamos esta red).
- **WEP**: Codificación muy básica ya obsoleta. Es muy fácil obtener la clave mediante programas o incluso intentos de “fuerza bruta” (cuestión de minutos), se desaconseja su uso. De todas formas, al menos es un poco más segura que la abierta.
- **WPA**: Codificación más complicada. De todas formas, hoy en día es hackeable, aunque requiere mucho más tiempo que la WEP (horas). Es preferible adquirir un punto de acceso o router que ofrezca el siguiente nivel de seguridad.
- **WPA2**: Más complicado de obtener la clave, si se toman las precauciones básicas es muy complicado de hackear (días o semanas seguidas) aunque sería siempre posible obtenerla. Será interesante complementar este nivel de protección (por ahora el más elevado). 


## Consejos de seguridad en redes Wifi domésticas

!!! tip "Cambio de SSID"
    El nombre de la red que emitimos (WLAN_23 por ejemplo) es recomendable cambiarlo, dado que ofrece pistas de la MAC de la tarjeta de red del router. De aquí, un potencial intruso podría sacar con una fórmula matemática (en un programa informático) la clave de encriptación WPA o WEP en segundos…. Con WPA2 es más difícil. Se recomienda poner un nombre neutral (que no produzca interés en los potenciales intrusos de la zona).


!!! tip "Cambio de clave de acceso a la WIFI"
    Requisito casi imprescindible y que hoy en día te sugiere el instalador. Se recomienda una clave con letras mayúsculas y minúsculas, con números y con algún signo de puntuación (:-.,;!/) para complicar la vida a intentos de “fuerza bruta”.

!!! tip "Cambio de clave de acceso al router"
    Requisito muy recomendable para que un intruso no nos destruya la conexión o se la apropie. Se pueden usar las claves generadas como en el apartado anterior. Si el router lo permite, es recomendable cambiar el usuario también.

!!! tip "Conexión por WPS"
    Sin dar la clave a nadie, se puede conectar un dispositivo (móvil, tablet, ordenador) a nuestro router utilizando el botón de WPS. Cuantas menos personas conocen la clave, mejor (los amigos de mis amigos no tienen porqué ser mis amigos, en contra de lo que dice la canción).

!!! tip "Ocultación de SSID"
    Se puede hacer oculto el nombre de la red wifi. De esta forma, si no se saben el nombre de nuestra red no podrán ni siquiera intentar sacar la clave. Existen maneras de averiguar la SSID aunque esté oculta, pero no son obvias y son imposibles en algunos dispositivo. Complementa la seguridad anterior.

!!! tip "Direccionamiento IP fijo (deshabilitar DHCP)"
    A cada ordenador le asignamos una dirección para siempre. Esto se puede hacer del lado del ordenador (aunque otra persona podría intentar arrebatarnos esta IP) o desde el router, con un tiempo de préstamo de la IP casi infinito. De esta forma es más complicado que puedan conectar a través de nuestro router, pero tiene formas de ser evitado.


!!! tip "Filtrado de equipos por MAC"
    El método más seguro en general es permitir únicamente a los equipos que conozcamos y sepamos su MAC. Aunque también se puede engañar al router, es más complicado y en algunos dispositivos más (móviles, por ejemplo).


## Factores que influyen en la velocidad de conexión a Internet

La velocidad máxima de una conexión está limitada por la velocidad más lenta de todos los pasos entre el inicio y el fin. Veamos los pasos: 

1. Del ordenador al switch: si es por cable, o 100 Mbps o 10 Mbps. Si es inalámbrico, depende de la distancia y de la tecnología de la antena wifi. En Wifi-n, el límite teórico es 150 Mbps, en Wifi-G es 54 Mbps, pero cae rápidamente. 
2. Del switch al router. Normalmente no hay problema, o va por cable (100 Mbps) o está en el mismo aparato. 
3. Router: puede estar “colgado” por exceso de conexiones o mucho tiempo encendido. 
4. Conexión contratada: de la velocidad que te prometen dependiendo del contrato te queda una parte garantizada (premium el 80%, 8 Mbps, línea de usuario 50 %...). 
5. La calidad de cobre ADSL desde centralita a tu casa. En El Casar la velocidad máxima era de 20 Mbps. En caso de la fibra óptica, esto no suele introducir error. 
6. Congestión en la red: esto sólo pueden arreglarlo los operadores de la red que tengas contratada. 
7. La velocidad de subida del equipo al que nos conectamos dividida entre los que quieren conectarse (por ejemplo, si [www.marca.es](www.marca.es) tuviera sólo 100 Mbps de subida para repartir entre todos las personas que acceden a su página de inicio a la vez podría darse lentitud en el acceso si varios intentan conectar a la vez. Si fueran sólo 1000 usuarios, ya estarían limitados a 100 kbps máximo). En general, los servidores más visitados suelen estar preparados para estas circunstancias contratando más capacidad (les interesa para poder cobrar más por publicidad dar cabida a más usuarios).