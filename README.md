# springboot-helm-chart

Further information in blog article [Spring Boot Applications with Helm](https://blog.viadee.de/en/spring-boot-applications-with-helm).

## Install/uninstall chart

The helm chart can be installed through a helm chart repository hosted on a GitHub page in this repository. To install or deinstall follow the steps:

```shell
helm repo add viadee https://viadee.github.io/springboot-helm-chart
export helm_release_name="viadeeExampleApplication"
helm install $helm_release_name viadee/springboot-helm-chart

# uninstall
helm delete $helm_release_name
```

The delete command removes all the Kubernetes resources associated with the chart and deletes the release.
