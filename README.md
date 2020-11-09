## Example Frontend/Backend deployment

Creates a DeploymentConfig, Service, and ImageStream for a frontend and backend application. Sets up a PostgresDB. And Puts the services behind an OAuth proxy using Keycloak as a security realm.

Also sets up a Tekton pipeline

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


