## Example Frontend/Backend deployment

Creates a DeploymentConfig, Service, Route, and ImageStream for a backend application. 

#### Update Helm Dependencies

```
helm dependency update
```

#### Install Helm Chart

```
helm install . --name-template <TEMPLATE_NAME> --namespace <namespace> --create-namespace
```

### Update Helm Chart to newer version

Update `appVersion` in the `Chart.yaml` file

```
helm upgrade <TEMPLATE_NAME> .
```


