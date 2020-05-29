Enable ingress on microk8s
```sh
microk8s enable ingress
```

Add basic auth
```sh
htpasswd -c auth will
kubectl create secret generic basic-auth --from-file=auth
```

Add TLS cert
```sh
kubectl create secret tls willstoney-tls --key willstoney.key --cert willstoney.crt
```