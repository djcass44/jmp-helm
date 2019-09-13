# JMP

[JMP](https://github.com/djcass44/jmp) is an open source application for quickly navigating to websites & addresses.

## Introduction

This chart deploys a JMP instance. It does NOT provide a database.

## Prerequisites

- Kubernetes 1.6+
- A JDBC compatible database (otherwise JMP will default to SQLite)
- An unused PersistentVolumeClaim

## Installing the chart

To install the chart:

```shell script
helm package jmp-helm
helm install jmp-helm-X.X.X.tgz
```

The above configuration deploys JMP on the Kubernetes cluster in its default configuration.

## Uninstalling the chart

To uninstall/delete the deployment:

```bash
$ helm list
NAME       	REVISION	UPDATED                 	STATUS  	CHART          	NAMESPACE
kindly-newt	1       	Mon Oct  2 15:05:44 2017	DEPLOYED	sonarqube-0.1.0	default
$ helm delete kindly-newt
```

## Configuration

See [values.yaml](values.yaml) for configuration options.