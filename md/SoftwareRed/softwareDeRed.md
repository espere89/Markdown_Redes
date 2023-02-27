# Software de red
---

## PDU (Paquetes de información) 

La información se codifica en binario y se manda en paquetes (PDU). Consta de las siguientes partes:
- Header (cabecero), con la información básica (como un sello con remitente y destino)
- Payload (carga o mensaje) es el contenido en bruto. Estos paquetes pueden estar cifrados o sólo llevar cifrada la información.

## Protocolos 

Para poder comunicarse entre sí se usan los *protocolos*. Son normas que regulan de qué forma se codifica la información (a nivel electrónico). Se comunican siempre a niveles distintos. Hay máquinas que se dedican a pasar entre niveles distintos. Estos niveles se llaman la PILA OSI.

<figure markdown>
  ![Imatge 6](../../img/imatge3.png){ width="400" }
  <figcaption>Pila OSI</figcaption>
</figure> 




Cada capa se dedica a los siguientes pasos en la comunicación:

| Nivel | Funciones |
| :---: | :--- |
| 1 Físico | Configuración pines y niveles de voltaje |
| 2 Ligado | HDLC/LAPB Determinación de marcos, checqueo de errores, intercambio de reconocimiento |
| 3 Red | Enrutado de paquetes, ensamblado de marcos, conexión del nodo a la red |
| 4 Transporte | Comunicación nodo a nodo, chequeo de errores |
| 5 Sesión | Servicio de PAD: Conexión de una terminal a un nodo central pod medio de dialup |
| 6 Presentación | Compresión de texto, transmisión de imágenes, ASN |
| 7 Aplicación | Aplicación |

La pila OSI es teórica, en el caso de TCP/IP (que es el que analizaremos más en profundidad) son menos capas. Veamos un gráfico más detallado de los niveles de ambos modelos:

<figure markdown>
  ![Imatge 7](../../img/imatge4.png){ width="500" }
  <figcaption>Capas modelo OSI y TCP/IP</figcaption>
</figure> 




Hay muchos protocolos importantes que controlan el paso de información. Algunos importantes:

- **HTTP:** protocolo usado en páginas web y que se basa en hipervínculos. 

- **HTTPS:** lo mismo pero seguro. Usa conexiones codificadas. 

- **FTP:** protocolo de transferencia de archivos, poco segura pero rápida. 

- **UDP:** User Datagram Protocol, para completar la velocidad en descargas P2P. Veloz pero nada seguro (se pueden perder datos). 

- **VoIP:** Voz sobre IP, se usa únicamente a la transmisión de sonido (voz) a través de Internet. En la actualidad, también se usa para la línea normal de teléfono porque es mucho más barata para la compañía operadora. 

- **TCP/IP:** El protocolo más importante es el TCP/IP. TCP significa Protocolo de Control de Transmisión, que indica que se controla los dos extremos de una comunicación (si están activos, la velocidad, el equipo al que van dirigidos...). La ventaja principal es el control para mantener viva la comunicación incluso si no hay datos. La transmisión de datos se realiza por paquetes de datos (PDU), que son conjuntos de ceros y unos “encapsulados” como si fueran cajas unas dentro de otras con etiquetas. Estos paquetes permiten saber a quién pertenecen los datos y devolverlos al usuario correcto.