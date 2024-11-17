# k8s

## Create a pod
```
kubectl run nginx --image=nginx
```

### Create a pod with a service
```
kubectl run nginx --image=nginx --port=80 --expose=true
```

## Create a yaml
```
Kubectl run redid —image=redis124 —dry-run -o yaml
```

## Create a service
Create a Service named redis-service of type ClusterIP to expose pod redis on port 6379

kubectl expose pod redis --port=6379 --name redis-service --dry-run=client -o yaml


## Imperative commands
```
kubectl create deployment <NAME> --image=<IMAGE> --replicas=3
```

## Certification Tip: Formatting Output with kubectl

kubectl [command] [TYPE] [NAME] -o <output_format>

Here are some of the commonly used formats:

`-o json` Output a JSON formatted API object.

`-o name`Print only the resource name and nothing else.

`-o wide` Output in the plain-text format with any additional information.

`-o yaml` Output a YAML formatted API object.

## Shortcuts
`rs`: ReplicaSet

`po`: Pod

`deploy`: Deployment

`svc`: Service

`ns`: Namespace

`no`: Node

`cm`: ConfigMap

`sec`: Secret

`pv`: PersistentVolume

`pvc`: PersistentVolumeClaim

`sa`: ServiceAccount

`ing`: Ingress

`job`: Job

`cronjob`: CronJob
