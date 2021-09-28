# helm-repository
My helm chart repository

## Install chart

```bash
helm install -n databases mongo ./mongo --create-namespace --set mongo.USERNAME=<username> --set mongo.PASSWORD=<password>
```

## Remove chart

```bash
helm uninstall -n databases monogo
```

## Dry Run

Try out the templating with a dry run

```bash
clear && helm install -n databases  --debug --dry-run mongo ./charts/mongo
```