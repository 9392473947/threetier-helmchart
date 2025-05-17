To run database from first we need to add repo for bitnami

helm repo add bitnami https://charts.bitnami.com/bitnami
helm repo update


helm install my-postgres bitnami/postgresql \
--set auth.username=cruduser \
--set auth.password=password \
--set auth.database=cruddb

then install backend and frontend charts...
