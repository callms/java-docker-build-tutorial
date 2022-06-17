# java-docker-build-tutorial

This is a sample project that shows how to deploy a basic Java app on an EKS cluster.

It is very basic, and inspired from https://github.com/miguno/java-docker-build-tutorial

## Steps

### EKS

Make sure you have a valid EKS cluster.

### Prepare the files for your environment

Copy the files from `sample` on the root directory, and edit them to change the AWS account to your own (the files have been written for account 834843395643, perform a search and replace).

### Deploy on your cluster

```bash
kubectl apply -f java-docker-build-tutorial.yaml
```

### Profit

Make sure the service is deployed:

```bash
kubectl get all
```
