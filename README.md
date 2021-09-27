# Helm Ian Teda

A collection of helm charts for Kubernetes deployments.

## Using this Helm Repository

This repository can be added to your Helm register by running the `helm repo add` command.

```bash
helm repo add ian-teda https://ianteda.github.io/helm-ian-teda/
```

Once the repository is added a chart can be installed with the `install` command.

```bash
helm install -n databases databases ian-teda/database --create-namespace
```

## How to Host Your Own Helm repo

### Create a Helm chart

Create a new helm chart with the `create` command.

```bash
helm create charts/redis
```

### Lint the Charts

To check your chart run the `lint` command on your chart.

```bash
helm lint charts/redis
```

### Create the Helm chart package

Once you are happy with the chart create the tgz package with the `package` command.

```bash
helm package charts/redis
```

### Add new chart

After you have packaged up your chart it can be added to the repository index with the `repo` command.

```bash
helm repo index --url https://ianteda.github.io/helm-ian-teda/ --merge index.yaml .
```
