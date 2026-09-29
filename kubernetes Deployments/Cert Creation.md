# How *seti.com* certificate was created

==Reference==
	==Server: setihost - 172.20.4.50==
	==Folder:  /home/setiadmin/tls-certs==

Cert-Commands:
```bash unwrap:true title:"Sequence of commands for self-signing root certificate"
openssl req -x509 -nodes -new -sha256 -days 3650 -newkey rsa:2048 \
	  -keyout myLocalCA.key \
	  -out myLocalCA.crt \
	  -subj "/CN=Seti Local Root CA"
	  
openssl genrsa -out tls.key 2048

openssl req -new -key tls.key -out server.csr -subj "/CN=*.seti.com"

openssl x509 -req -in server.csr \
  -CA myLocalCA.crt -CAkey myLocalCA.key -CAcreateserial \
  -out tls.crt -days 365 -sha256 -extfile v3.ext

```


```bash unwrap:true title:"Kubernetes secret commands"
kubectl get secrets -n keycloak-ns

kubectl delete secret keycloak-tls-secret -n keycloak-ns

kubectl create secret tls keycloak-tls-secret --cert=tls.crt --key=tls.key -n keycloak-ns

```
