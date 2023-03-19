# podman-compose-cookbook

A Podman version of [docker-compose-cookbook](https://github.com/aaronchenwei/docker-compose-cookbook).

## Prerequisite

- [Podman](https://podman.io/)
- [Podman Compose](https://github.com/containers/podman-compose)

For AlmaLinux 9, we can simply install them through

```sh
$ sudo dnf install podman podman-compose
```

## How to Use

```sh
$ podman-compose up -d
```

### To Migrate to Kubernetes Pods

```sh
$ podman ps

$ podman generate kube -f nexus.yaml b4fdcb0709e1
# with Kube Service 
$ podman generate kube -s -f nexus.yaml b4fdcb0709e1
```
