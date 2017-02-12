# Jump-Start Go (JustGo)

Skeleton project for jump-starting a Go-powered microservice development with Docker and Go best-practices.

To learn more: [https://justgo.rocks](https://justgo.rocks)

## How to run:

1. Install a working Docker environment
    1. Mac: https://docs.docker.com/docker-for-mac/
    2. Windows: https://docs.docker.com/docker-for-windows/
    3. Linux: https://docs.docker.com/engine/installation/linux/
2. cd to the project's root folder and run `docker-compose build --no-cache` (optional but good step)
3. In the same folder, run: `docker-compose up -d`
4. If you get a clean output, you can check which port the server
   attached to by running: `docker-compose ps`
4. For instance, if the output was: `0.0.0.0:32791` under `ports` section then you
   can access your new service at `http://0.0.0.0:32791/`
5. You can edit source files of the application without restarting anything
   since JustGo supports hot reloading, using [Gin](https://github.com/codegangsta/gin)

## Stopping and removing

While in the project folder:

```
> docker-compose stop 
> docker-compose rm -f 
```

## License

[MIT](LICENSE)