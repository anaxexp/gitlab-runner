# Gitlab Runner Docker Container Image 

[![Build Status](https://travis-ci.org/anaxexp/gitlab-runner.svg?branch=master)](https://travis-ci.org/anaxexp/gitlab-runner)
[![Docker Pulls](https://img.shields.io/docker/pulls/anaxexp/gitlab-runner.svg)](https://hub.docker.com/r/anaxexp/gitlab-runner)
[![Docker Stars](https://img.shields.io/docker/stars/anaxexp/gitlab-runner.svg)](https://hub.docker.com/r/anaxexp/gitlab-runner)
[![Docker Layers](https://images.microbadger.com/badges/image/anaxexp/gitlab-runner.svg)](https://microbadger.com/images/anaxexp/gitlab-runner)

## Overview

This gitlab runner image registers on CI server automatically when `CI_SERVER_URL` and `REGISTRATION_TOKEN` specified.

## Docker Images

!!! For better reliability we release images with stability tags (`anaxexp/gitlab-runner:10-X.X.X`) which correspond to [git tags](https://github.com/anaxexp/gitlab-runner/releases). We **STRONGLY RECOMMEND** using images only with stability tags. 

Overview:

* All images are based on Alpine Linux
* Base image: [gitlab/gitlab-runner](https://hub.docker.com/r/gitlab/gitlab-runner/)
* [Travis CI builds](https://travis-ci.org/anaxexp/gitlab-runner) 
* [Docker Hub](https://hub.docker.com/r/anaxexp/gitlab-runner)

Supported tags and respective `Dockerfile` links:

* `10`, `10.4`, `latest` [_(Dockerfile)_](ttps://github.com/anaxexp/gitlab-runner/tree/master/Dockerfile)

## Environment Variables

| Variable             | Default Value            | Description |
| -------------------- | ------------------------ | ----------- |
| `RUNNER_EXECUTOR`    | `docker`                 |             |
| `DOCKER_IMAGE`       | `anaxexp/alpine:3.7-1.2.0` |             |
| `CI_SERVER_URL`      |                          |             |
| `REGISTRATION_TOKEN` |                          |             |

Run `gitlab-runner register --help` to see the full list of environment variables

## Deployment

Deploy GitLab runner to your own server via [![AnaxExp](https://www.google.com/s2/favicons?domain=anaxexp.com) AnaxExp](https://anaxexp.com).
