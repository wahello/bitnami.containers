# Percona XtraBackup packaged by Bitnami

## What is Percona XtraBackup?

> Percona XtraBackup is a set of tools for performing backups of MySQL databases. It executes online non-blocking, tightly compressed, and highly secure full backups on transactional systems.

[Overview of Percona XtraBackup](https://www.percona.com/software/mysql-database/percona-xtrabackup/)

Trademarks: This software listing is packaged by Bitnami. The respective trademarks mentioned in the offering are owned by the respective companies, and use of them does not imply any affiliation or endorsement.

## TL;DR

```console
$ docker run --name percona-xtrabackup bitnami/percona-xtrabackup:latest
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


* [`8`, `8-debian-11`, `8.0.28-21`, `8.0.28-21-debian-11-r16`, `latest` (8/debian-11/Dockerfile)](https://github.com/bitnami/bitnami-docker-percona-xtrabackup/blob/8.0.28-21-debian-11-r16/8/debian-11/Dockerfile)
* [`2.4`, `2.4-debian-11`, `2.4.26`, `2.4.26-debian-11-r16` (2.4/debian-11/Dockerfile)](https://github.com/bitnami/bitnami-docker-percona-xtrabackup/blob/2.4.26-debian-11-r16/2.4/debian-11/Dockerfile)

Subscribe to project updates by watching the [bitnami/percona-xtrabackup GitHub repo](https://github.com/bitnami/bitnami-docker-percona-xtrabackup).

## Get this image

The recommended way to get the Bitnami percona-xtrabackup Docker Image is to pull the prebuilt image from the [Docker Hub Registry](https://hub.docker.com/r/bitnami/percona-xtrabackup).

```console
$ docker pull bitnami/percona-xtrabackup:latest
```

To use a specific version, you can pull a versioned tag. You can view the [list of available versions](https://hub.docker.com/r/bitnami/percona-xtrabackup/tags/) in the Docker Hub Registry.

```console
$ docker pull bitnami/percona-xtrabackup:[TAG]
```

If you wish, you can also build the image yourself.

```console
$ docker build -t bitnami/percona-xtrabackup:latest 'https://github.com/bitnami/bitnami-docker-percona-xtrabackup.git#master:8/debian-11'
```

## Configuration

### Running commands

To run commands inside this container you can use `docker run`. The container has the Percona XtraBackup tools `xtrabackup`, `xbstream`, `xbcrypt` and `xbcloud`. For example, to run `xtrabackup --version` you can follow the example below:

```console
$ docker run --rm --name percona-xtrabackup bitnami/percona-xtrabackup:latest -- xtrabackup --version
```

Check the [official percona-xtrabackup documentation](https://www.percona.com/doc/percona-xtrabackup/LATEST/manual.html) for a list of the available parameters.

## Contributing

We'd love for you to contribute to this container. You can request new features by creating an [issue](https://github.com/bitnami/bitnami-docker-percona-xtrabackup/issues), or submit a [pull request](https://github.com/bitnami/bitnami-docker-percona-xtrabackup/pulls) with your contribution.

## Issues

If you encountered a problem running this container, you can file an [issue](https://github.com/bitnami/bitnami-docker-percona-xtrabackup/issues/new). For us to provide better support, be sure to include the following information in your issue:

- Host OS and version
- Docker version (`docker version`)
- Output of `docker info`
- Version of this container
- The command you used to run the container, and any relevant output you saw (masking any sensitive information)

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
