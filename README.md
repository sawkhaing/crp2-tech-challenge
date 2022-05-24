
# k8s-helm

This is a simple application deployment in kubernetes, it's configured to work.

Please find the base code under [k8s-helm]](k8s-helm)

```
helm upgrade -n interview --install --values k8s-helm/helm/values.yaml interview-task k8s-helm/helm/
```

The application is working by taking value of env variable `WORLD` to display the output on webpage.

## Questions

1. This deployment is currently not working properly, can you figure out why.
2. Add the necessary code to expose this service to outside of the cluster. Also, when querying different endpoints it should show each of the different services you created on the previous step:
   - `http://<address>/de` should show "Hello Freund"
   - `http://<address>/es` should show "Hello Amigo"
   - `http://<address>/fr` should show "Hello Ami"
   - other endpoint should show "Hello Friend"
