Remote Desktop Protocol Protocolo de Escritorio Remoto es un protocolo propietario desarrollado por Microsoft que permite la comunicación en la ejecución de una aplicación entre una terminal y un servidor Windows

## Funcionamiento

El modo de funcionamiento del protocolo es sencillo. La información gráfica que genera el servidor es convertida a un formato propio RDP y enviada a través de la red al terminal, que interpretará la información contenida en el paquete del protocolo para reconstruir la imagen a mostrar en la pantalla del terminal. En cuanto a la introducción de órdenes en el terminal por parte del usuario, las teclas que pulse el usuario en el teclado del terminal así como los movimientos y pulsaciones de ratón son redirigidos al servidor, permitiendo el protocolo un cifrado de los mismos por motivos de #seguridad. El #protocolo también permite que toda la información que intercambien cliente y [[servidor]] sea comprimida para un mejor rendimiento en las redes menos veloces.

Este servicio utiliza por defecto el puerto `TCP 3389` en el servidor para recibir las peticiones. Una vez iniciada la sesión desde un punto remoto el ordenador servidor mostrará la pantalla de bienvenida de windows, no se verá lo que el usuario está realizando de forma remota.

Este servicio tiene distintos tipos de aplicaciones: se utiliza frecuentemente para el acceso remoto en la administración de equipos, pero también es cada vez más utilizado en la gestión de servicios de terminal o clientes ligeros "Cliente ligero" (_thin clients_).