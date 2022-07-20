# Envoy packaged by Bitnami

## What is Envoy?

> Envoy is a distributed, high-performance proxy for cloud-native applications. It features a small memory footprint, universal application language compatibility, and supports http/2 and gRPC.

[Overview of Envoy](https://www.envoyproxy.io/)

Trademarks: This software listing is packaged by Bitnami. The respective trademarks mentioned in the offering are owned by the respective companies, and use of them does not imply any affiliation or endorsement.

## TL;DR

```console
$ docker run --name envoy bitnami/envoy:latest
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


* [`1.22`, `1.22-debian-11`, `1.22.2`, `1.22.2-debian-11-r13`, `latest` (1.22/debian-11/Dockerfile)](https://github.com/bitnami/bitnami-docker-envoy/blob/1.22.2-debian-11-r13/1.22/debian-11/Dockerfile)
* [`1.21`, `1.21-debian-11`, `1.21.4`, `1.21.4-debian-11-r12` (1.21/debian-11/Dockerfile)](https://github.com/bitnami/bitnami-docker-envoy/blob/1.21.4-debian-11-r12/1.21/debian-11/Dockerfile)
* [`1.20`, `1.20-debian-11`, `1.20.6`, `1.20.6-debian-11-r9` (1.20/debian-11/Dockerfile)](https://github.com/bitnami/bitnami-docker-envoy/blob/1.20.6-debian-11-r9/1.20/debian-11/Dockerfile)
* [`1.19`, `1.19-debian-11`, `1.19.5`, `1.19.5-debian-11-r13` (1.19/debian-11/Dockerfile)](https://github.com/bitnami/bitnami-docker-envoy/blob/1.19.5-debian-11-r13/1.19/debian-11/Dockerfile)

Subscribe to project updates by watching the [bitnami/envoy GitHub repo](https://github.com/bitnami/bitnami-docker-envoy).

## Get this image

The recommended way to get the Bitnami envoy Docker Image is to pull the prebuilt image from the [Docker Hub Registry](https://hub.docker.com/r/bitnami/envoy).

```console
$ docker pull bitnami/envoy:latest
```

To use a specific version, you can pull a versioned tag. You can view the [list of available versions](https://hub.docker.com/r/bitnami/envoy/tags/) in the Docker Hub Registry.

```console
$ docker pull bitnami/envoy:[TAG]
```

If you wish, you can also build the image yourself.

```console
$ docker build -t bitnami/envoy:latest 'https://github.com/bitnami/bitnami-docker-envoy.git#master:1.22/debian-11'
```

## Configuration

### Running commands

To run commands inside this container you can use `docker run`, for example to execute `envoy --version` you can follow the example below:

```console
$ docker run --rm --name envoy bitnami/envoy:latest -- --version
```

Check the [official envoy documentation](https://www.envoyproxy.io/docs/envoy/latest/operations/cli) for a list of the available parameters.

### Adding your custom configuration

By default, envoy will look for a configuration file in `/opt/bitnami/envoy/conf/envoy.yaml`. You can launch the envoy container with your custom configuration with the command below:

```console
$ docker run --rm -v /path/to/your/envoy.yaml:/opt/bitnami/envoy/conf/envoy.yaml bitnami/envoy:latest
```

Visit the [official envoy documentation](https://www.envoyproxy.io/docs/envoy/latest/configuration/configuration) for all the available configurations.

## Contributing

We'd love for you to contribute to this container. You can request new features by creating an [issue](https://github.com/bitnami/bitnami-docker-envoy/issues), or submit a [pull request](https://github.com/bitnami/bitnami-docker-envoy/pulls) with your contribution.

## Issues

If you encountered a problem running this container, you can file an [issue](https://github.com/bitnami/bitnami-docker-envoy/issues/new). For us to provide better support, be sure to include the following information in your issue:

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
