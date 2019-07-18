# wordpress-kubernetes
# Inatall Wordpress On Kubernetes 


* # Configure a MySQL database
create a secret password for the MySQL root user

`kubectl create secret generic mysql-pass --from-literal=password=MYSQL_ROOT_PASSWORD`


