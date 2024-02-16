# Kinbaku Server

## Installation

```console
$ git clone --recurse-submodules ...  # clone this repo, INCLUDING sub repos
$ cp env.default .env  # copy default configuration
$ nano .env  # adjust configuration for your use case
$ docker-compose up -d  # run production and development server
```

## Deploy updates

After changes to the submodule kinbaku, to deploy changes to development:

```console
$ (cd kinbaku-dev && git pull)
$ docker-compose build
$ docker-compose up -d
```

To deploy changes to production:

```console
$ (cd kinbaku && git pull)
$ docker-compose build
$ docker-compose up -d
```


