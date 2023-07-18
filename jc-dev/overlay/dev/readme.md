# How to Use Custom Error Pages

```
$ kubectl edit -n ingress-nginx cm ingress-nginx-controller

# add custom-http-errors: "503" as part of its data field

$ kubectl edit -n ingress-nginx deploy/ingress-nginx-controller

# add --default-backend-service=jc-dev/nginx-errors as part of its args

# save
```