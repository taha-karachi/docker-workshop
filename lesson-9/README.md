# Docker Compose
Just like `Dockerfile` makes creating images easier, Docker Compose makes deploying containers easier.

Docker Compose expects a YAML file, usually named `docker-compose.yml`, which contains information about what image to use to run containers.

It let you run multiple containers as one service.

## Installing Docker Compose
You have to download it separately, as it does not come with Docker.

```bash
$ sudo curl -L https://github.com/docker/compose/releases/download/1.21.1/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose
```

The above long command downloads and installs `docker-compose` to `/usr/local/bin`.

## Networks
In the previous lesson, we only created single containers. To be specific a web server, which in the real-world does not makes sense if your website is dynamic.

There has to be a database or other services running along with the web server to make a useful application.

> TODO: Complete this lesson