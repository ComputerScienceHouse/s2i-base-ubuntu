# Ubuntu S2I Base Docker Image

This repository contains a Dockerfile that serves as the base image with all essential libraries and tools needed for OpenShift language images, namely:

* [s2i-swift](https://github.com/ComputerScienceHouse/s2i-swift)

## Installation and Usage

This image is available on DockerHub. To pull it, run:

```
docker pull computersciencehouse/base-ubuntu16.04
```

To build the base image from scratch, run:

```
git clone https://github.com/ComputerScienceHouse/s2i-base-ubuntu.git
cd s2i-base-ubuntu
make build
```

## Test

This repository includes the S2I test framework, which launches a simple test to make sure the image builds and runs properly.

```
cd s2i-base-ubuntu
make test
```
