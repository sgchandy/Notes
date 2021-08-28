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
 
  
  
kubectl create -f replicaset-def.yaml
  
kubectl get replicaset
  
kubectl describe replicaset <name>

kubectl delete replicaset myapp-replicaset
  
kubectl replace -f replicaset-def.yml
  
kubectl scale --replicas=6 -f replicaset-def.yml
  
kubectl scale replicaset myapp-replicaset --replicas=6
  
kubectl edit replicaset myapp-replicaset

  

kubectl create deployment <name> --image=<image_name>
  
kubectl describe deployment <name>
 
  
  


![image](https://user-images.githubusercontent.com/45700418/131227130-015e92e7-66bd-47d3-8656-6633deb7b39e.png)

  
Difference in yaml (Deployment vs ReplicaSet)
  
  ![image](https://user-images.githubusercontent.com/45700418/131227262-49089462-8d51-4422-ad0f-aeb0325027ce.png)




  ![image](https://user-images.githubusercontent.com/45700418/131228010-6739c3e4-8288-4667-9df8-1de21edbed94.png)

  
  
  ![image](https://user-images.githubusercontent.com/45700418/131227931-6198ef64-a606-453e-8554-fa4db62ebb68.png)


  
  ![image](https://user-images.githubusercontent.com/45700418/131227946-b9c7ced6-af74-4e15-a9f4-2896415f312b.png)

  
  
  ![image](https://user-images.githubusercontent.com/45700418/131228924-d7a6d230-7ab3-444b-af82-a2d441099f49.png)

  
  
![image](https://user-images.githubusercontent.com/45700418/131229525-59768bcc-c678-44c1-9011-efddc717c1eb.png)
  
![image](https://user-images.githubusercontent.com/45700418/131229533-0b2777c7-d942-4907-834d-7e7d80bafc04.png)
  

  
  
  ![image](https://user-images.githubusercontent.com/45700418/131229645-3e835ef7-2088-4850-aca1-421b50be7c20.png)

  
