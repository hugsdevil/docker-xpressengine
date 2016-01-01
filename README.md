# Table of Contents
- [Introduction](#introduction)
  - [Version](#version)
  - [Changelog](Changelog.md)
- [Specification](#specification)
  - [Minimum Requirement](#minimum-requirement)
  - [Test Enviroment](#test-enviroment)
- [Installation](#installation)
  - [Quick Start](#quick-start)
  - [Configuration](#configuration)
    - [Database](#database)
      - [MySQL](#mysql)
- [Contribution](#contribution)
- [Issues](#issues)
- [Reference](#reference)

# Introduction
Dockerfile to build a xpressengine container image.

## Version
Latest version xe-1.8.3.

# Specification

## Minimum Requirements
None.

## Test Enviroments
- CPU : Intel Atom D2700
- Memory : Samsung Notebook DDR3 4G PC3-8500
- Disk : WD Red 4TB WD40EFRX (SATA3/64M)
- OS : Linux 3.10.35
- Docker : 1.6.2
- Etc : Synology DS412+

# Installation

## Quick Start
```bash
docker run -d --name xe -p 80:80 registry.hub.docker.com/hugsdevil/xpressengine:latest
```

Alternately you can build the image locally.

```bash
git clone https://github.com/hugsdevil/docker-xpressengine.git
cd docker-xpressengine
docker build --tag="my-image-name" .
```

## Configuration

### Database

#### MySQL
- Create ID, Password, DB for xe
- IP 172.17.42.1 (https://docs.docker.com/articles/networking/)
- PORT 3306

# Contribution
If you find this image useful here's how you can help:

- Send a Pull Request with your awesome new features and bug fixes
- Help new users with [Issues](https://github.com/hugsdevil/docker-xpressengine/issues) they may encounter

# Issues
Issue for xpressengine.

- Unknown download naming for xe version
- Configuration problem for DB, User, etc
- Add plugin

# References
- Dockerfile (https://github.com/docker-library/wordpress/blob/master/apache/Dockerfile)
- README.md (https://github.com/sameersbn/docker-gitlab/blob/master/README.md#version)
