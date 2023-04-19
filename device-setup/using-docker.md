# Using Docker

You'll need any computer with an Operaying System that can run [Docker](https://www.docker.com/) & [docker-compose](https://docs.docker.com/get-started/08\_using\_compose/). You might need someone with technical skills on these tools to set it up.

Using Docker EDT-Offline can be setup in almost any machine without any special operating system needed.

Needed installed software

* [Docker](https://www.docker.com/)
* [docker-compose](https://docs.docker.com/get-started/08\_using\_compose/)
* [git](https://git-scm.com/downloads)

These are the steps:

1. Clone repository
2. cd `docker/local` directory
3. `cp .env.example .env`
4. Edit `.env` with your own values
5. Run `docker-compose up -d`
6. Use `docker-compose logs -f` to see logs
