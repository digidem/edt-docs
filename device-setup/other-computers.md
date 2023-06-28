# Computadoras regulares

En las máquinas regulares, el proceso es similar al de formatear cualquier otra computadora. Se realiza mediante el parpadeo de una unidad USB y obteniendo que esta arranque a través de comandos del teclado.

**Dispositivos recomendados:**

* [Zimaboard 432](https://shop.zimaboard.com/products/zimaboard-single-board-server-for-creators-8g-32gb-linux-windows-openwrt-pfsense-andorid-libreelec-development-board-low-cost-hackable-single-board-server)

#### Hardware necesario

* Cualquier computadora antigua con almacenamiento que se pueda formatear, como máquinas de escritorio o portátiles antiguas con disco duro o SSD con al menos 30 GB de almacenamiento
* Cualquier unidad USB con al menos 2 GB de almacenamiento
* Conexión a Internet a través de un cable Ethernet
* Teclado
* Monitor y cables

#### Software necesario

* Grabador de imágenes, recomendado: [Balena Etcher](https://www.balena.io/etcher/)

#### Preparando la unidad de flash USB

Descargue y utilice la imagen **Generic x86\_64 (GPT)** para máquinas AMD regulares en: [http://releases.earthdefenderstoolkit.com](http://releases.earthdefenderstoolkit.com/)

Utilice el grabador de imágenes para grabar la imagen en la unidad de flash USB.

#### Instalando la herramienta sin conexión a internet

* Inserte la unidad USB con el sistema en la computadora
* Inserte el cable Ethernet con Internet proveniente de su enrutador en la computadora
* Descubra cómo activar el menú de arranque o cómo ingresar a la BIOS y ajustar el orden de arranque
* Seleccione que el arranque se realice a través de UEFI o USB, y el dispositivo debería comenzar la configuración
* La configuración puede tardar varios minutos dependiendo de la capacidad de la computadora&#x20;
* Verifique el [Panel de control de Balena](https://dashboard.balena-cloud.com/) para que el dispositivo esté en línea, o verifique si ha aparecido un nuevo punto de acceso WiFi
* En caso de que haya pasado mucho tiempo sin que ocurra nada, desconecte y vuelva a conectar el suministro de energía.

En caso de tener problemas con su configuración, consulte la sección de [solución de problemas](troubleshooting.md "mention"). Si todo funcionó, consulte [sincronización-de-contenido.md](../device-usage/first-steps/syncing-content.md "mention") para obtener contenido en su nueva herramienta sin conexión a internet.