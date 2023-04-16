```bash
helm repo add k8s-helm-phonebookrepo https://raw.githubusercontent.com/yavuz69/k8s-helm-phonebookrepo/main
helm install phonebook-app k8s-helm-phonebookrepo/phonebook-chart
```

- To use own images execute as below:

```bash
helm install phonebook-app k8s-helm-phonebookrepo --set webserver_image=<image-name> --set resultserver_image=<image-name>
```