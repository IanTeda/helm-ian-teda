# helm-repository
My helm chart repository

## Install chart

```bash
clear && helm install -n admin heimdall ./charts/heimdall --create-namespace
```

## Remove chart

```bash
helm uninstall -n downloaders heimdall
```

## Dry Run

Try out the templating with a dry run

```bash
clear && helm install -n downloaders  --debug --dry-run heimdall ./charts/heimdall
```

## Reference

* [Docker Instructions](https://heimdall.tv/#downloads-v3-docker)
* [linuxserver/heimdall](https://docs.linuxserver.io/images/docker-heimdall)