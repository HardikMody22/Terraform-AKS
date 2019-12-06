# Terraform-AKS
Deploying from dockerhub to AKS using terraform

## Steps To Deploy
### az login
### az ad sp create-for-rbac -n "MyApp"
### terraform init
### terraform plan
### terraform graph | dot -Tsvg > graph.svg (Optional)
### terraform apply
### Use Azure Client_ID and Client_Secret
### kubectl version
### terraform output kube_config > ~/.kube/config-terraform-aks-demo
### export KUBECONFIG=~/.kube/config-terraform-aks-demo:~/.kube/config
### echo "export KUBECONFIG=${KUBECONFIG}" >> ${HOME}/.bash_profile
### kubectl get nodes
### kubectl version
### kubectl apply -f mydeploy.yaml
### kubectl get pods
### kubectl apply -f myservice.yaml
### kubectl get svc
### See the external_ip and type it in the browser
### kubectl get pods
### kubectl delete pod <georgemichael-86fd69d65-2wrjf>
### kubectl delete pod <georgemichael-86fd69d65-txzwb>
### Won't be deleted since you haven't deleted deployment
### kubectl get pods
### kubectl delete deployment <georgemichael>
### kubectl get services
### kubectl delete service <georgemichael>
### kubectl delete service <kubernetes>
### terraform destroy
### kubectl get services
