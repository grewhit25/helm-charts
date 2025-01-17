# transmission

![Version: 0.2.5](https://img.shields.io/badge/Version-0.2.5-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 3.00](https://img.shields.io/badge/AppVersion-3.00-informational?style=flat-square)

A Fast, Easy, and Free BitTorrent Client.

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://nicholaswilde.github.io/helm-charts/ | common | ~0.1.5 |

## TL;DR
```console
$ helm repo add nicholaswilde https://nicholaswilde.github.io/helm-charts/
$ helm repo update
$ helm install transmission nicholaswilde/transmission
```

## Installing the Chart
To install the chart with the release name `transmission`:
```console
helm install transmission nicholaswilde/transmission
```

## Uninstalling the Chart
To uninstall the `transmission` deployment:
```console
helm uninstall transmission
```
The command removes all the Kubernetes components associated with the chart and deletes the release.

## Configuration

Read through the [values.yaml](./values.yaml) file. It has several commented out suggested values.
Other values may be used from the [values.yaml](../common/values.yaml) from the [common library](../common).

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`. For example,
```console
helm install transmission \
  --set env.TZ="America/New York" \
    nicholaswilde/transmission
```

Alternatively, a YAML file that specifies the values for the above parameters can be provided while installing the chart.
For example,
```console
helm install transmission nicholaswilde/transmission -f values.yaml
```

## Author
This project was started in 2020 by [Nicholas Wilde](https://github.com/nicholaswilde).

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.4.0](https://github.com/norwoodj/helm-docs/releases/v1.4.0)
