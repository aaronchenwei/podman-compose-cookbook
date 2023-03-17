# podman-compose-cookbook

A podman version of [docker-compose-cookbook](https://github.com/aaronchenwei/docker-compose-cookbook)

## Prerequisite

- podman
- podman compose

For AlmaLinux 9, we can simply install them through

```sh
$ sudo dnf install podman podman-compose
```

## How to Use

```sh
$ podman-compose up -d

# to migrate to kube
$ podman ps

$ podman generate kube -f nexus.yaml b4fdcb0709e1
# with Service 
$ podman generate kube -s -f nexus.yaml b4fdcb0709e1
```

