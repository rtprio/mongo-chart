# amazee.io mongodb chart

# usage

1. verify uids in `values.yaml`
1. run

       helm install --name mongodb1 -f values.yaml stable/mongodb-replicaset --namespace mongodb

## Dependency: Tiller

1. If helm/tiller is not installed make sure tiller server is installed by following https://blog.openshift.com/getting-started-helm-openshift/

> Note: tiller requires admin cluster role. Add it with:

       oc adm policy add-cluster-role-to-user cluster-admin system:serviceaccount:tiller:tiller
