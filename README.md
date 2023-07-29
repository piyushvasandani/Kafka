# Setting up a kafka cluster
## Step-1: Go inside the directory
```
cd Kafka-cluster
```
## Step-2: Creating Resources In Kubernetes
```
kubectl create -f statefulset-zookeeper.yaml
kubectl create -f headless-service-zookeeper.yaml
kubectl create -f statefulset-multi-broker-kafka-with-zk.yaml
kubectl create -f kafka-0-service.yaml
kubectl create -f kafka-1-service.yaml
kubectl create -f kafka-2-service.yaml
kubectl create -f headless-service-kafka.yaml
kubectl create -f bootstrap-service-kafka.yaml
```
