# Kuberentes Service Account 

# steps 

1 # created a namespace cloud-engeering 
2 # created a service cloud-engineer in cloud-engineering ns
3 # created internal-app deployment - updated to use serviceAccount & ns to cloud-engineering 

# verification: 

# kubectl get pods -n cloud-engineering 
# NAME                            READY   STATUS    RESTARTS   AGE
# internal-app-6c68fdb678-hsc5d   1/1     Running   0          7m24s


# kubectl describe pod internal-app -n cloud-engineering | grep Service 
# Service Account:  cloud-engineers