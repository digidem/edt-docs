---
descripción: ¿Cuáles son las habilidades técnicas básicas necesarias para esta configuración?
---

# Introducción

> ⚠️ Tenga en cuenta que durante la versión beta, confiamos en el servicio Balena Cloud de una empresa, y tienen puertas traseras para todos los dispositivos.&#x20;

El proceso para preparar un dispositivo para ejecutar la Earth Defenders Offline Toolkit requiere una computadora portátil o de escritorio, utilizada para "quemar" imágenes en tarjetas SD o unidades flash USB. Por lo tanto, se requieren habilidades básicas para su uso.

Para obtener ayuda con problemas técnicos comunes, consulte la sección [troubleshooting.md](troubleshooting.md "mencionada") de esta guía. Para obtener ayuda adicional, consulte la sección [support.md](../support.md "mencionada").

### Diferentes procesos

Cualquier vieja computadora puede ser reciclada para ejecutar el software stack de Earth Defenders Offline Toolkit. Idealmente, debería formatear las máquinas antiguas para ejecutar nuestro sistema operativo ligero, consulte [other-computers.md] (other-computers.md "mencionado").

La Toolkit sin conexión también puede ejecutar los servicios junto con su sistema operativo existente, consulte [using-docker.md](using-docker.md "mencionado"). Este proceso no está respaldado y está desconectado de Balena Cloud, por lo que respeta la soberanía de los datos.

Si la intención es comprar un nuevo dispositivo con este propósito, le recomendamos que compre una computadora de una sola tarjeta, ya que tienden a ser más baratas, más móviles, consumen menos energía y son más fáciles de configurar, consulte [single-board-computers.md](single-board-computers.md "mencionado").

### Instalaciones compatibles

El equipo de Digital Democracy tendrá acceso al dispositivo y a todos los datos, pero no accederá ni extraerá datos sin consentimiento. Monitorearemos los dispositivos en busca de problemas de software y hardware, para que podamos brindar soporte.

Pero la compañía Balena también tendrá acceso a las puertas traseras del dispositivo, que probablemente no se usarán, pero **pueden** usarse.

Actualmente generamos imágenes de soporte listas para usar que se pueden grabar en cualquier computadora regular y en determinadas computadoras de tablero único seleccionadas.

Para ver todas las imágenes de modo de soporte lanzadas, visite: [http://releases.earthdefenderstoolkit.com](http://releases.earthdefenderstoolkit.com/) ".Continúa hacia [choosing-a-device.md](choosing-a-device.md "mención") para encontrar el dispositivo que mejor se adapte a tus necesidades.

### Instalaciones no compatibles

El proceso es muy similar al proceso compatible, pero en lugar de descargar nuestra imagen, crearás la tuya usando Balena Cloud. Haz clic en [aquí](https://dashboard.balena-cloud.com/deploy?repoUrl=https://github.com/digidem/edt-offline) y Balena te guiará por el proceso.

Generarás tu propia imagen, pero ejecutando nuestro software. De esta manera, podrás administrar tu propio conjunto de dispositivos.

Revisa [connecting-to-the-internet.md](../device-usage/first-steps/connecting-to-the-internet.md "mención") y [syncing-content.md](../device-usage/first-steps/syncing-content.md "mención") para aprender cómo obtener el contenido de tu kit sin conexión.

Aún necesitarás ponerte en contacto con nosotros, al menos para autorizar la sincronización del contenido, consulta [support.md](../support.md "mención").