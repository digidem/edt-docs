# Servicios 

## Syncthing 

Es una aplicación gratuita de sincronización de archivos entre pares, de código abierto, disponible para la mayoría de las plataformas. Puede sincronizar archivos entre dispositivos en una red local o entre dispositivos remotos a través de Internet. La seguridad y la protección de los datos están integradas en el diseño del software. Es una alternativa FOSS a [Resilio Sync](https://www.resilio.com).

La aplicación se utiliza para mantener actualizado el contenido (mapas de configuración y tiles, sitios web sin conexión, repositorio f-droid, etc.) disponible cuando los dispositivos de la comunidad u organización se conecten a internet.

El saludo inicial entre la instancia en la nube y otros dispositivos se inicia automáticamente por el dispositivo EDT Offline, pero necesita ser aceptado por alguien con acceso al servicio en la Nube.

## Navegador de archivos

Ofrece una interfaz de gestión de archivos dentro de un directorio especificado y se puede utilizar para cargar, eliminar, previsualizar, renombrar y editar archivos. Permite la creación de varios usuarios y cada usuario puede tener su propio directorio. Se puede utilizar como una aplicación independiente. Es una alternativa FOSS a Google Drive, sin las suites de oficina.\*\*\*\*

Se utiliza para navegar por el contenido tanto en la nube como en el dispositivo sin conexión. El equipo que ofrece soporte a las comunidades debe utilizarlo para agregar o eliminar contenido que se hospeda en la nube. Los dispositivos sin conexión pueden usarlo para compartir archivos con el equipo de soporte o dentro de la red local.

## Repositorio F-Droid 

F-Droid es una tienda de aplicaciones y un repositorio de software para Android. Las aplicaciones se pueden navegar, descargar e instalar desde la aplicación cliente sin la necesidad de registrarse para obtener una cuenta. Es una alternativa FOSS a la tienda Google Play.

Hemos bifurcado una aplicación cliente y creado nuestro propio cliente [EDT Apps](https://github.com/digidem/edt-apps), que viene con nuestro propio [repositorio de aplicaciones EDT](https://github.com/digidem/edt-fdroid-repository), así como con el repositorio que se ejecuta en los dispositivos EDT sin conexión.Los clientes regulares de F-Droid también pueden hacer uso del repositorio EDT simplemente agregando la URL a su lista de repositorios o escaneando el código QR presentado.

## Sala de Secure Scuttlebut

La aplicación principal del cliente, [Manyverse] (https://www.manyver.se/), es una red social sin cosas malas, construida sobre el protocolo SSB punto a punto. Es gratuita y de código abierto, y está disponible para escritorio y móvil. No se ejecuta en la nube propiedad de una empresa, en su lugar, todos los datos viven completamente en los dispositivos de los usuarios. De esta manera, incluso fuera de línea, los usuarios pueden desplazarse, leer cualquier cosa e incluso escribir publicaciones y gustar el contenido. Cuando el dispositivo vuelve a estar en línea, sincroniza las últimas actualizaciones directamente con otros dispositivos, a través de una red Wi-Fi local compartida o en Internet.

La Sala SSB es un servicio que permite a los pares "conocerse" en línea e intercambiar datos. Al ejecutar nuestra propia Sala, podemos conectar a los socios entre sí y también ofrecer soporte a los equipos. Tiene funciones de gestión de usuarios (roles de autorización y denegación de permisos + moderador y administrador) todos administrados a través del panel web.

## Almacenamiento de Minio

MinIO es una solución de almacenamiento de objetos de alto rendimiento que proporciona una API compatible con Amazon Web Services S3 y admite todas las funciones principales de S3. Es una alternativa de código abierto a Amazon S3.

Se utiliza para organizar los datos de Terrastories en cubos. De esta manera, si un socio desea que sus Terrastories se publiquen en la nube, podemos sincronizar su cubo Minio, que se ejecuta en el dispositivo Offline de EDT, y ejecutar una instancia de Terrastories en la nube extrayendo datos de eso. Proporciona una forma organizada de mantener en sincronía las instancias de Terrastories en línea y sin conexión.