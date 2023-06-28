# Dispositivos de desarrollo

### Túnel hacia un dispositivo de desarrollo

Para facilitar la depuración y realizar pruebas de control de calidad en una función o una liberación, es útil exponer los servicios del dispositivo virtual. Podemos hacer uso de [tailscale](https://tailscale.com) para eso.

Inicie sesión por SSH en el dispositivo virtual Balena utilizando el **UUID**, el cual se puede obtener en el panel de control de Balena:

`balena ssh <uuid>`

Dentro del entorno virtual Balena, ejecute:

```
balena run -d \
    --name=tailscaled \
    --restart always \
    -e TS_STATE_DIR=/var/lib/tailscale \
    -v tailscale-state:/var/lib/tailscale \
    -v /dev/net/tun:/dev/net/tun \
    --network=host \
    --privileged \
    tailscale/tailscale tailscaled
```

Y para comenzar el servicio de **tailscale**, ejecute:

```
balena exec tailscaled tailscale up --advertise-routes=10.0.3.0/24 --accept-routes --reset
```

El contenedor de Tailscale le proporcionará una URL para acceder que agrega el dispositivo a su cuenta de Tailscale.

Luego [habilite las subredes](https://tailscale.com/kb/1019/subnets/#step-3-enable-subnet-routes-from-the-admin-console) desde su panel de administración de Tailscale para poder utilizar todos los dispositivos localmente a través de las direcciones IP que les asigna Balena Virt.

En su propio dispositivo ejecute:

```
docker run -d \
    --name=tailscaled \
    --restart always \
    -e TS_STATE_DIR=/var/lib/tailscale \
    -v tailscale-state:/var/lib/tailscale \
    -v /dev/net/tun:/dev/net/tun \
    --network=host \
    --privileged \
    tailscale/tailscale tailscaled
```

Y para iniciar Tailscale:

```
docker exec tailscaled tailscale up --advertise-routes=10.0.3.0/24 --accept-routes --reset
```

No olvide habilitar también las subredes. Ahora en su dispositivo debería poder acceder a los servicios a través de la dirección IP del dispositivo Balena.

### Usando el dispositivo remoto

Para que Terrastories y el mapa sin conexión en Terrastories y Observations Map funcionen de forma remota, debe establecer las variables del dispositivo para utilizar la dirección IP tunelizada:

* `HOST_HOSTNAME` ej.: 100.96.14.113".* `OFFLINE_MAP_STYLE` por ejemplo: http://100.96.14.113:8085/styles/terrastories-map/style.json

### Configurando una máquina virtual

Lea los detalles en el [repositorio oficial](https://github.com/balena-labs-research/balena-virt).

Asegúrese de tener una flota Balena con **generic x86\_64 (GPT)** como el **Dispositivo predeterminado**.

En un droplet de Digital Ocean con al menos 25 GB de almacenamiento, 1 GB de RAM y la última versión de Docker preinstalada, ejecute:

```
docker run -it \
    -d \
    --restart always \
    -v bv_pid:/app/pid \
    --device=/dev/kvm \
    --cap-add=net_admin \
    -e API_TOKEN="your_balena_token" \
    -e FLEET="your_balena_fleet" \
    -e MEM=1024M \
    -e DISK=20G \
    -e DEV_MODE=true \
    --network host \
    ghcr.io/balena-labs-research/balena-virt:latest
```

Después de unos segundos, debería aparecer un nuevo dispositivo en su amd64 y debería comenzar a actualizarse con la última versión para la flota.