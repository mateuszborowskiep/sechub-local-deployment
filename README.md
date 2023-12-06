# Description
Local deployment of SecHub mercedes security tool with Kubernetes with separate psql database services, replicaset and pods 

# Declarative deploy
kubectl apply -f deployment.yaml -f networkpolicy.yaml -f secrets.yaml -f service.yaml  

# Debugging
kubectl get pods 
kubectl describe <pod>
kubectl logs <pod>

# Clean up 
kubectl delete -f deployment.yaml -f networkpolicy.yaml -f secrets.yaml -f service.yaml  

# TD
Add PDS server with separate deployment 