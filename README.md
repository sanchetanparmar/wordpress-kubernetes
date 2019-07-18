# wordpress-kubernetes
# Inatall Wordpress On Kubernetes 


* # Configure a MySQL database
 * create a secret password for the MySQL root user

`kubectl create secret generic mysql-pass --from-literal=password=MYSQL_ROOT_PASSWORD`

* Create Volumes

`kubectl apply -f volumes.yml`

* Create Mysql Deployment and Service

`kubectl apply -f mysql.yml`

* Create Worepress Deployment and Service

`kubectl apply -f wordpress.yml`


As Wordpres Services hosted on `NodePort - nodePort: 30001` you can get wp installation page 


```http://HostIP:30001```



