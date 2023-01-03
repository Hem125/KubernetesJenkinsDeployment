# KubernetesJenkinsDeployment

Downgrading the version

sudo kubeadm reset
sudo apt-get purge kubeadm kubectl kubelet kubernetes-cni kube*  
sudo apt-get autoremove  
sudo rm -rf ~/.kube


How to taint when we need to schedule opposed of node affinity 

kubectl taint node AMANTYA_VM node-role.kubernetes.io/master-

Nodes to schedule 
kubectl get nodes -o json | jq '.items[].spec.taints'

Kubernetes Credential 

Manage Jenkins and than Manage Credential 

![image](https://user-images.githubusercontent.com/103022040/210328347-859d5a39-4a11-4e32-9a85-6b202f247d7e.png)

Go to .kube and  copy config file  upload as a secret file 

![image](https://user-images.githubusercontent.com/103022040/210328596-3fe9d666-5fb0-46d7-9d39-b7c8c04c4f62.png)






