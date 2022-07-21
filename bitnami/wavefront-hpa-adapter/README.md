# Wavefront HPA Adapter for Kubernetes

## What is Wavefront HPA Adapter for Kubernetes?

> Wavefront HPA Adapter for Kubernetes is a Kubernetes Horizontal Pod Autoscaler adapter. It allows to scale your Kubernetes workloads based on Wavefront metrics.

[Overview of Wavefront HPA Adapter for Kubernetes](https://github.com/wavefrontHQ/wavefront-kubernetes-adapter)



## TL;DR

```console
$ docker run --name wavefront-hpa-adapter bitnami/wavefront-hpa-adapter:latest
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


* [`0`, `0-scratch`, `0.9.9`, `0.9.9-scratch-r0`, `latest` (0/scratch/Dockerfile)](https://github.com/bitnami/bitnami-docker-wavefront-hpa-adapter/blob/0.9.9-scratch-r0/0/scratch/Dockerfile)

Subscribe to project updates by watching the [bitnami/wavefront-hpa-adapter GitHub repo](https://github.com/bitnami/bitnami-docker-wavefront-hpa-adapter).

## Get this image

The recommended way to get the Bitnami wavefront-hpa-adapter Docker Image is to pull the prebuilt image from the [Docker Hub Registry](https://hub.docker.com/r/bitnami/wavefront-hpa-adapter).

```console
$ docker pull bitnami/wavefront-hpa-adapter:latest
```

To use a specific version, you can pull a versioned tag. You can view the [list of available versions](https://hub.docker.com/r/bitnami/wavefront-hpa-adapter/tags/) in the Docker Hub Registry.

```console
$ docker pull bitnami/wavefront-hpa-adapter:[TAG]
```

If you wish, you can also build the image yourself.

```console
$ docker build -t bitnami/wavefront-hpa-adapter:latest 'https://github.com/bitnami/bitnami-docker-wavefront-hpa-adapter.git#master:0/scratch'
```

## Why use a non-root container?

Non-root container images add an extra layer of security and are generally recommended for production environments. However, because they run as a non-root user, privileged tasks are typically off-limits. Learn more about non-root containers [in our docs](https://docs.bitnami.com/tutorials/work-with-non-root-containers/).

## Configuration

### Running commands

To run commands inside this container you can use `docker run`, for example to execute `wavefront-adapter --wavefront-url example.wavefront.com` you can follow the example below:

```console
$ docker run --rm --name wavefront-hpa-adapter bitnami/wavefront-hpa-adapter:latest --  --wavefront-url example.wavefront.com
```

Check the [official Wavefront HPA Adapter for Kubernetes documentation](https://github.com/wavefrontHQ/wavefront-kubernetes-adapter/blob/master/docs/configuration.md) for a list of the available parameters.

## Contributing

We'd love for you to contribute to this container. You can request new features by creating an [issue](https://github.com/bitnami/bitnami-docker-wavefront-hpa-adapter/issues), or submit a [pull request](https://github.com/bitnami/bitnami-docker-wavefront-hpa-adapter/pulls) with your contribution.

## Issues

If you encountered a problem running this container, you can file an [issue](https://github.com/bitnami/bitnami-docker-wavefront-hpa-adapter/issues/new). For us to provide better support, be sure to include the following information in your issue:

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
