# helm-repository
My helm chart repository

## Install chart

```bash
helm install -n databases postgres ./charts/postgres --create-namespace /
  --set auth.username=<username> \
  --set auth.password=<password>
```

## Remove chart

```bash
helm uninstall -n databases postgres
```

## Dry Run

Try out the templating with a dry run

```bash
helm install -n databases postgres ./charts/postgres --create-namespace /
  --set auth.username=<username> \
  --set auth.password=<password> \
  --debug --dry-run
```