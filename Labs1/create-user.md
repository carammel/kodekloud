## Create certificate and private key for user
openssl genrsa -out  mike.key 2048
openssl req -new -key mike.key -out mike.csr -subj "/CN=mike/O=dev"

It is important to set CN and O attribute of the CSR. CN is the name of the user and O is the group that this user will belong to. You can refer to RBAC for standard groups.
## 

https://collabnix.com/how-to-create-user-in-kubernetes-cluster-and-give-it-access/ 
