
 de Transferencia de Hipertexto)

### Introducción
___

### La Web

Internet (o La Web) es es un sistema de información de cliente/servidor distribuido masivamente como se muestra en el siguiente diagrama. 

![alt text](https://www.ntu.edu.sg/home/ehchua/programming/webprogramming/images/TheWeb.png)

Muchas aplicaciones se están ejecutando al mismo tiempo en la web, tales como la navegación web, e-mail, transferencias de archivos, transmisión de audio y vivo, entre otros. Para lograr una correcta comunicación entre el cliente y el servidor, esas aplicaciones deben estar en un mismo nivel de protocolo tales como HTTP, FTP, SMTP, POP, etc.

### Protocolo de Transferencia de Hipertexto (HTTP)
HTTP (Protocolo de  Transferencia de Hipertexto) es probablemente el protocolo de aplicación mas usado en Internet (La Web).

* HTTP es un protocolo cliente-servidor asimétrico de solicitud-respuesta como se ilustra. Un cliente HTTP envía una solicitud a un servidor HTTP. El servidor, a su vez, regresa un mensaje de respuesta. En otras palabras, HTTP es un protocolo de extracción, el cliente extrae información del servidor (en lugar de que el servidor arroje información al cliente).

![alt text](https://www.ntu.edu.sg/home/ehchua/programming/webprogramming/images/HTTP.png)

* HTTP es un protocolo sin estado. En otras palabras, la solicitud actual no sabe que es lo que se ha hecho en las solicitudes anteriores.

* HTTP permite la negociación del tipo de datos y la representación, con el fin de permitir que los sistemas sean construidos independientemente de los datos que se transfieren. 

* Citando el RFC2616: "El Protocolo de Transferencia de Hyper Texto es un protocolo de nivel de aplicación para sistemas de colaboración, información hipermedia distribuidos. Es un protocolo genérico, sin estados el cual puede ser usado para muchas tareas mas allá de su uso para hipertenso, tales como servidores de nombres y sistemas de gestión de objetos distribuidos, mediante de la extensión de sus métodos de solicitudes, códigos de error y cabeceras"

### Navegador

Cada vez que se ejecuta una URL desde tu navegador para obtener un recurso web usando HTTP, ej. http://www.nowhere123.com/index.html, el navegador convierte la URL en un mensaje de solicitud y lo envía al servidor HTTP. El servidor HTTP interpreta el mensaje de solicitud, y regresa un mensaje de respuesta apropiado, el cual es el recurso que solicitaste o un mensaje de error. Este proceso se ilustra abajo: 

![alt text](https://www.ntu.edu.sg/home/ehchua/programming/webprogramming/images/HTTP_Steps.png)

### Localizador Uniforme de Recursos (URL)

Un URL (Localizador Uniforme de Recursos) es usa para identificar de forma única un recurso a través de internet. URL tiene la siguiente sintaxis:
```
protocolo://nombre-del-host:puerto/ruta-y-nombre-de-archivo
```

Hay 4 partes en un URL
	1. *Protocolo*: El protocolo de nivel de aplicación usado por el cliente y servidor, ej., HTTP, FTP, y telnet.
