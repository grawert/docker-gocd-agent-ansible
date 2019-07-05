# GoCD Agent Docker image with Ansible

The image is based on [gocd-agent-ubuntu-18.04](https://hub.docker.com/r/gocd/gocd-agent-ubuntu-18.04)
and Ansible is installed additionally.

## Requirements

- Docker

## Setup

    docker pull ugrawert/gocd-agent-ubuntu-18.04-ansible

## Run

    docker run --rm -d -e GO_SERVER_URL=https://go-server:8154/go -v $PWD/config:/godata ugrawert/gocd-agent-ubuntu-18.04-ansible
