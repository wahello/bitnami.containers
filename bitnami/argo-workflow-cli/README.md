# Argo Workflows packaged by Bitnami

## What is Argo Workflows?

> Argo Workflows is meant to orchestrate Kubernetes jobs in parallel. It uses DAG and step-based workflows

[Overview of Argo Workflows](https://argoproj.github.io/workflows)

Trademarks: This software listing is packaged by Bitnami. The respective trademarks mentioned in the offering are owned by the respective companies, and use of them does not imply any affiliation or endorsement.

## TL;DR

```console
$ docker run -it --name argo-workflow-cli bitnami/argo-workflow-cli
```

### Docker Compose

```console
$ curl -sSL https://raw.githubusercontent.com/bitnami/bitnami-docker-argo-workflow-cli/master/docker-compose.yml > docker-compose.yml
$ docker-compose up -d
```

## Why use Bitnami Images?

* Bitnami closely tracks upstream source changes and promptly publishes new versions of this image using our automated systems.
* With Bitnami images the latest bug fixes and features are available as soon as possible.
* Bitnami containers, virtual machines and cloud images use the same components and configuration approach - making it easy to switch between formats based on your project needs.
* All our images are based on [minideb](https://github.com/bitnami/minideb) a minimalist Debian based container image which gives you a small base container image and the familiarity of a leading Linux distribution.
* All Bitnami images available in Docker Hub are signed with [Docker Content Trust (DCT)](https://docs.docker.com/engine/security/trust/content_trust/). You can use `DOCKER_CONTENT_TRUST=1` to verify the integrity of the images.
* Bitnami container images are released on a regular basis with the latest distribution packages available.

## How to deploy Argo Workflows CLI in Kubernetes?

Deploying Bitnami applications as Helm Charts is the easiest way to get started with our applications on Kubernetes. Read more about the installation in the [Bitnami Argo Workflows Chart GitHub repository](https://github.com/bitnami/charts/tree/master/bitnami/argo-workflows).

## Why use a non-root container?

Non-root container images add an extra layer of security and are generally recommended for production environments. However, because they run as a non-root user, privileged tasks are typically off-limits. Learn more about non-root containers [in our docs](https://docs.bitnami.com/tutorials/work-with-non-root-containers/).

## Supported tags and respective `Dockerfile` links

Learn more about the Bitnami tagging policy and the difference between rolling tags and immutable tags [in our documentation page](https://docs.bitnami.com/tutorials/understand-rolling-tags-containers/).


* [`3`, `3-scratch`, `3.3.8`, `3.3.8-scratch-r5`, `latest` (3/scratch/Dockerfile)](https://github.com/bitnami/bitnami-docker-argo-workflows/blob/3.3.8-scratch-r5/3/scratch/      Dockerfile)

Subscribe to project updates by watching the [bitnami/argo-workflow-cli GitHub repo](https://github.com/bitnami/bitnami-docker-argo-workflow-cli).

## Get this image

The recommended way to get the Bitnami Argo Workflows CLI Docker Image is to pull the prebuilt image from the [Docker Hub Registry](https://hub.docker.com/r/bitnami/argo-workflow-cli).

```console
$ docker pull bitnami/argo-workflow-cli:latest
```

To use a specific version, you can pull a versioned tag. You can view the [list of available versions](https://hub.docker.com/r/bitnami/argo-workflow-cli/tags/) in the Docker Hub Registry.

```console
$ docker pull bitnami/argo-workflow-cli:[TAG]
```

If you wish, you can also build the image yourself.

```console
$ docker build -t bitnami/argo-workflow-cli:latest 'https://github.com/bitnami/bitnami-docker-argo-workflow-cli.git#master:3/scratch'
```

## Maintenance

### Upgrade this image

Bitnami provides up-to-date versions of Argo Workflows CLI, including security patches, soon after they are made upstream. We recommend that you follow these steps to upgrade your container.

#### Step 1: Get the updated image

```console
$ docker pull bitnami/argo-workflow-cli:latest
```

or if you're using Docker Compose, update the value of the image property to `bitnami/argo-workflow-cli:latest`.

#### Step 2: Remove the currently running container

```console
$ docker rm -v argo-workflow-cli
```

or using Docker Compose:

```console
$ docker-compose rm -v argo-workflow-cli
```

#### Step 3: Run the new image

Re-create your container from the new image.

```console
$ docker run --name argo-workflow-cli bitnami/argo-workflow-cli:latest
```

or using Docker Compose:

```console
$ docker-compose up argo-workflow-cli
```

## Configuration

### Running commands

To run commands inside this container you can use `docker run`, for example to execute `argocd --help` you can follow the example below:

```console
$ docker run --rm --name argo-workflow-cli bitnami/argo-workflow-cli:latest --help
```

Check the [official Argo Workflows CLI documentation](https://argoproj.github.io/argo-workflows/cli/) for the list of the available parameters.

## Contributing

We'd love for you to contribute to this Docker image. You can request new features by creating an [issue](https://github.com/bitnami/bitnami-docker-argo-workflow-cli/issues), or submit a [pull request](https://github.com/bitnami/bitnami-docker-argo-workflow-cli/pulls) with your contribution.

## Issues

If you encountered a problem running this container, you can file an [issue](https://github.com/bitnami/bitnami-docker-argo-workflow-cli/issues/new). For us to provide better support, be sure to include the following information in your issue:

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
