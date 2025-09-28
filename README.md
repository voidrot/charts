# Voidrot Helm Charts

## Using this Repository as a Helm Chart Repo

This repository hosts Helm charts for deployment. You can use it as a Helm chart repository to install charts directly.

### Add the Helm Repository

```sh
helm repo add voidrot https://voidrot.github.io/charts/
helm repo update
```

### Install a Chart

List available charts:

```sh
helm search repo voidrot
```

Install a chart (replace `<chart-name>` and `<version>` as needed):

```sh
helm install my-release voidrot/<chart-name> --version <version>
```

### Example

```sh
helm repo add voidrot https://voidrot.github.io/charts/
helm repo update
helm install my-release voidrot/<chart-name>
```

---
For more details, see the [Helm documentation](https://helm.sh/docs/helm/helm_repo/).
