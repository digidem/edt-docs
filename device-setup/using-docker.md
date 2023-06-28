# Usando Docker

Necesitarás una computadora con un sistema operativo que pueda ejecutar [Docker](https://www.docker.com/) y [docker-compose](https://docs.docker.com/get-started/08_using_compose/). Es posible que necesites a alguien con habilidades técnicas en estas herramientas para configurarlas.

Usando Docker, EDT-Offline se puede configurar en casi cualquier máquina sin necesidad de un sistema operativo especial.

Software necesario instalado

* [Docker](https://www.docker.com/)
* [docker-compose](https://docs.docker.com/get-started/08_using_compose/)
* [git](https://git-scm.com/downloads)

Sigue estos pasos:

1. Clona el repositorio
2. Dirígete al directorio `docker/local`
3. `cp .env.example .env`
4. Edita `.env` con tus propios valores
5. Ejecuta `docker-compose up -d`
6. Usa `docker-compose logs -f` para ver los registros".