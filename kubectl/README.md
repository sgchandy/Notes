kubectl get all


kubectl get nodes
kubectl get nodes -o wide



kubectl get pods

kubectl get pods -o wide

kubectl describe pod <pod_name>

kubectl run <podman> --image <image>

kubectl create -f <filename.yaml>
  
kubectl apply -f <pods.yaml>

kubectl edit <pods_name>

kubectl delete pod <pod_name>

kubectl create deployment <name> --image=<image_name>

  
  
  
kubectl create -f replicaset-def.yaml
  
kubectl get replicaset

kubectl delete replicaset myapp-replicaset
  
kubectl replace -f replicaset-def.yml
  
kubectl scale --replicas=6 -f replicaset-def.yml
  
kubectl scale replicaset myapp-replicaset --replicas=6
  
kubectl edit replicaset myapp-replicaset



![image](https://user-images.githubusercontent.com/45700418/131227130-015e92e7-66bd-47d3-8656-6633deb7b39e.png)

  




