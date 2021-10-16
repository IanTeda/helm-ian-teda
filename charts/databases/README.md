# Databases Helm Chart

Set Chart dependencies in Chart.yaml

```yaml
...
dependencies:
  - name: redis
    version: 0.1.0
    repository: "https://ianteda.github.io/helm-ian-teda/"
  - name: postgres
    version: 0.1.0
    repository: "https://ianteda.github.io/helm-ian-teda/"
  - name: mongo
    version: 0.1.0
    repository: "https://ianteda.github.io/helm-ian-teda/"
  - name: elasticsearch
    version: 0.1.0
    repository: "https://ianteda.github.io/helm-ian-teda/"
```

Update chart dependencies

```bash
helm dep update charts/databases
```
