# Usando Balena Cloud



> &#x20;Una empresa externa administrará una plataforma de monitoreo para sus dispositivos, y tendrán puertas traseras a sus dispositivos.

Necesitará algún software para grabar imágenes en un dispositivo de almacenamiento (unidad flash o tarjeta SD), recomendamos [Balena Etcher] (https://www.balena.io/etcher/).

Cualquier persona puede implementar su propio EDT-Offline siguiendo estos pasos:

1. Haga clic en "[Implementar con Balena] (https://dashboard.balena-cloud.com/deploy?repoUrl=https://github.com/digidem/edt-offline) ”
2. Se le pedirá que cree una cuenta en Balena Cloud
3. Se le solicitará que implemente una nueva flota, cambie el nombre si es necesario y haga clic en "crear y implementar".
4. Haga clic en el botón "Agregar dispositivo"
5. Mantenga el modo "Producción" a menos que desee experimentar y tener acceso ssh al dispositivo.
6. Para configurar el dispositivo, necesitará Internet, elija la forma en que desea conectarse, ya sea a través de WiFi (proporcione las credenciales) o cable Ethernet.
7. Finalmente, haga clic en "Flash", que automáticamente flasheará usando Etcher, o usando la flecha, haga clic en "Descargar balenaOS", que descargará el archivo de imagen.
8. Inserte el almacenamiento en la computadora y grabe la imagen.
9. Finalmente inserte el almacenamiento en el dispositivo y observe su [Panel de control de Balena Cloud](https://dashboard.balena-cloud.com), debería aparecer un nuevo dispositivo y comenzar a actualizar su software.
10. Para sincronizar con el contenido predeterminado, deberá ponerse en contacto con nosotros por correo electrónico, Telegram o Whatsapp.

> &#x20;Cambie la ubicación del dispositivo en la pestaña "Ubicación" de Balena Cloud. Esto se recomienda si no desea que se encuentre su dispositivo en el [Balena Hub](https://hub.balena.io).