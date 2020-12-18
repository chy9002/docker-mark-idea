# docker-mark-idea

Build Mark-idea docker image for [Hansanshi/mark-idea](https://github.com/Hansanshi/mark-idea).

* You can run image with follow docker compose configure:

  ```yaml
  version: '3'
  services:
    mark-idea:
      image: chy9002/mark-idea
      ports:
        - "<host port>:8090"
      restart: always
      environment:
          - USERNAME=<default-username>
          - PASSWORD=<default-password>
      volumes:
              - <local_path>:/app/db
  ```

* Update image with `docker-compose pull`
* run container with `docker-composee up -d`
