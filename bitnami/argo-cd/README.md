# Argo CD packaged by Bitnami

## What is Argo CD?

> Argo CD is a continuous delivery tool for Kubernetes based on GitOps.

[Overview of Argo CD](https://argoproj.github.io/cd)

Trademarks: This software listing is packaged by Bitnami. The respective trademarks mentioned in the offering are owned by the respective companies, and use of them does not imply any affiliation or endorsement.

## TL;DR

```console
$ docker run -it --name argo-cd bitnami/argo-cd
```

### Docker Compose

```console
$ curl -sSL https://raw.githubusercontent.com/bitnami/bitnami-docker-argo-cd/master/docker-compose.yml > docker-compose.yml
$ docker-compose up -d
```

## Why use Bitnami Images?

* Bitnami closely tracks upstream source changes and promptly publishes new versions of this image using our automated systems.
* With Bitnami images the latest bug fixes and features are available as soon as possible.
* Bitnami containers, virtual machines and cloud images use the same components and configuration approach - making it easy to switch between formats based on your project needs.
* All our images are based on [minideb](https://github.com/bitnami/minideb) a minimalist Debian based container image which gives you a small base container image and the familiarity of a leading Linux distribution.
* All Bitnami images available in Docker Hub are signed with [Docker Content Trust (DCT)](https://docs.docker.com/engine/security/trust/content_trust/). You can use `DOCKER_CONTENT_TRUST=1` to verify the integrity of the images.
* Bitnami container images are released on a regular basis with the latest distribution packages available.

## Supported tags and respective `Dockerfile` links

Learn more about the Bitnami tagging policy and the difference between rolling tags and immutable tags [in our documentation page](https://docs.bitnami.com/tutorials/understand-rolling-tags-containers/).


* [`2`, `2-debian-11`, `2.4.7`, `2.4.7-debian-11-r3`, `latest` (2/debian-11/Dockerfile)](https://github.com/bitnami/bitnami-docker-argo-cd/blob/2.4.7-debian-11-r3/2/debian-11/      Dockerfile)

Subscribe to project updates by watching the [bitnami/argo-cd GitHub repo](https://github.com/bitnami/bitnami-docker-argo-cd).

## Get this image

The recommended way to get the Bitnami Argo CD Docker Image is to pull the prebuilt image from the [Docker Hub Registry](https://hub.docker.com/r/bitnami/argo-cd).

```console
$ docker pull bitnami/argo-cd:latest
```

To use a specific version, you can pull a versioned tag. You can view the [list of available versions](https://hub.docker.com/r/bitnami/argo-cd/tags/) in the Docker Hub Registry.

```console
$ docker pull bitnami/argo-cd:[TAG]
```

If you wish, you can also build the image yourself.

```console
$ docker build -t bitnami/argo-cd:latest 'https://github.com/bitnami/bitnami-docker-argo-cd.git#master:2/debian-11'
```

## Maintenance

### Upgrade this image

Bitnami provides up-to-date versions of Argo CD, including security patches, soon after they are made upstream. We recommend that you follow these steps to upgrade your container.

#### Step 1: Get the updated image

```console
$ docker pull bitnami/argo-cd:latest
```

or if you're using Docker Compose, update the value of the image property to `bitnami/argo-cd:latest`.

#### Step 2: Remove the currently running container

```console
$ docker rm -v argo-cd
```

or using Docker Compose:

```console
$ docker-compose rm -v argo-cd
```

#### Step 3: Run the new image

Re-create your container from the new image.

```console
$ docker run --name argo-cd bitnami/argo-cd:latest
```

or using Docker Compose:

```console
$ docker-compose up argo-cd
```

## Configuration

### Running commands

To run commands inside this container you can use `docker run`, for example to execute `argocd --help` you can follow the example below:

```console
$ docker run --rm --name argo-cd bitnami/argo-cd:latest --help
```

Check the [official Argo CD documentation](https://argo-cd.readthedocs.io/en/stable/operator-manual/server-commands/argocd-server/) for the list of the available parameters.

## Contributing

We'd love for you to contribute to this Docker image. You can request new features by creating an [issue](https://github.com/bitnami/bitnami-docker-argo-cd/issues), or submit a [pull request](https://github.com/bitnami/bitnami-docker-argo-cd/pulls) with your contribution.

## Issues

If you encountered a problem running this container, you can file an [issue](https://github.com/bitnami/bitnami-docker-argo-cd/issues/new). For us to provide better support, be sure to include the following information in your issue:

- Host OS and version
- Docker version (`docker version`)
- Output of `docker info`
- Version of this container
- The command you used to run the container, and any relevant output you saw (masking any sensitive
information)

## License

Copyright &copy; 2022 Bitnami

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
