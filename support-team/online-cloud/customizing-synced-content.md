# Personalizando contenido sincronizado

### 1. Extracción de información

La extracción de información de sitios web se realiza mediante el comando línea de comandos [browsertrix-crawler](https://github.com/webrecorder/browsertrix-crawler). Puede encontrar más instrucciones en la [documentación de rastreo](https://www.notion.so/Web-Crawling-c8f980b0fac54cdc9c2d9a308461ddd9).

Se requiere experimentación para encontrar las mejores prácticas para obtener exactamente la cantidad de páginas que deseamos extraer, y para cada idioma.

La extracción de información puede tardar mucho tiempo. Use los archivos warcz de salida en el siguiente paso.

### 2. Subir a la nube

Diríjase al servicio [FileBrowser](https://files.earthdefenderstoolkit.com) en la nube de EDT.

<figure><img src="../../.gitbook/assets/Untitled.png" alt=""><figcaption></figcaption></figure>

Existen diferentes directorios dentro del directorio `content`, cada uno para un tipo de contenido: datos de repositorios F-Droid; instaladores de escritorio; datos Mapeo (configs y tiles); y sitios web sin conexión.

Cree una nueva carpeta para su nuevo contenido si es necesario:

Asegúrese de que haya suficiente almacenamiento disponible en el servidor y, para cargar nuevo contenido, simplemente arrástrelo a la carpeta o use el ícono de carga para seleccionar el archivo de su ordenador:

<figure><img src="../../.gitbook/assets/Untitled 1 (1).png" alt=""><figcaption></figcaption></figure>

Una vez que se haya cargado el nuevo contenido, podemos sincronizarlo con los dispositivos de EDT.

### 3. Sincronización

Diríjase al servicio [Syncthing](http://sync.earthdefenderstoolkit.com/) en la nube de EDT y siga los mismos pasos que en [content-syncronization.md](../../device-usage/bundled-applications/content-syncronization.md "mención").

### 4. Añadir al dispositivo

Consulte las instrucciones en [syncing-content.md](../../device-usage/first-steps/syncing-content.md "mención") sobre cómo comenzar a sincronizar con un nuevo dispositivo. Deberá conseguir su ID Syncthing.

En la instancia de EDT Cloud, busque esa ID:



<figure><img src="../../.gitbook/assets/Untitled 6 (1).png" alt=""><figcaption></figcaption></figure>

Proporcione un nombre descriptivo para el nuevo dispositivo e ir a la página **Compartir**:"<figure><img src="../../.gitbook/assets/Untitled 7.png" alt=""><figcaption></figcaption></figure>

En la página de **Compartir**, selecciona todas las carpetas relevantes para el nuevo dispositivo, por lo general las predeterminadas:

<figure><img src="../../.gitbook/assets/Untitled 8 (1).png" alt=""><figcaption></figcaption></figure>

En EDT Cloud deberías ver que el dispositivo comienza a sincronizarse:

<figure><img src="../../.gitbook/assets/Untitled 9.png" alt=""><figcaption></figcaption></figure>

En la herramienta Offline Toolkit local también deberías ver la sincronización en progreso con más detalles como la velocidad de descarga y la cantidad sincronizada hasta ahora.

Listo. Ahora cada vez que la carpeta de contenido de Cloud se actualice, los dispositivos Offline Toolkit se sincronizarán automáticamente cada vez que estén en línea."