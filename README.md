# springboot-helm-chart

## Install/deinstall chart

The helm chart can be installed through a helm chart repository hosted on a GitHub page in this repository. To install or deinstall follow the steps:

```shell
helm repo add viadee https://viadee.github.io/springboot-helm-chart
export helm_release_name="viadeeExampleApplication"
helm install $helm_release_name viadee/springboot-helm-chart

# deinstall
helm delete $helm_release_name
```

The delete command removes all the Kubernetes resources associated with the chart and deletes the release.
