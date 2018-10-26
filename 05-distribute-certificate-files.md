> Move certificate files to the worker nodes:

```
scp ca.pem <worker 1 hostname>-key.pem <worker 1 hostname>.pem user@<worker 1 public IP>:~/
scp ca.pem <worker 2 hostname>-key.pem <worker 2 hostname>.pem user@<worker 2 public IP>:~/
```

> Move certificate files to the controller nodes:

```
scp ca.pem ca-key.pem kubernetes-key.pem kubernetes.pem \
    service-account-key.pem service-account.pem user@<controller 1 public IP>:~/
scp ca.pem ca-key.pem kubernetes-key.pem kubernetes.pem \
    service-account-key.pem service-account.pem user@<controller 2 public IP>:~/
```
