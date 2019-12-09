# Terraform-AKS
Deploying from dockerhub to AKS using terraform

## Kindly use the Raw Format

## Steps To Deploy
### 1. az login
### 2. az ad sp create-for-rbac -n "MyApp"
### 3. terraform init
### 4. terraform plan
### 5. terraform graph | dot -Tsvg > graph.svg (Optional)
### 6. terraform apply
#### Use Azure Client_ID and Client_Secret
### 7. kubectl version
### 8. terraform output kube_config > ~/.kube/config-terraform-aks-demo
### 9. export KUBECONFIG=~/.kube/config-terraform-aks-demo:~/.kube/config
### 10. echo "export KUBECONFIG=${KUBECONFIG}" >> ${HOME}/.bash_profile
### 11. kubectl get nodes
### 12. kubectl version
### 13. kubectl apply -f mydeploy.yaml
### 14. kubectl get pods
### 15. kubectl apply -f myservice.yaml
### 16. kubectl get svc
#### See the external_ip and type it in the browser
### 17. kubectl get pods
### 18. kubectl delete pod <georgemichael-86fd69d65-2wrjf>
### 19. kubectl delete pod <georgemichael-86fd69d65-txzwb>
#### Won't be deleted since you haven't deleted deployment
### 20. kubectl get pods
### 21. kubectl delete deployment <georgemichael>
### 22. kubectl get services
### 23. kubectl delete service <georgemichael>
### 24. kubectl delete service <kubernetes>
### 25. terraform destroy
### 26. kubectl get services
