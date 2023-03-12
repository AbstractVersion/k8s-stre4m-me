## coresplain vs teraform
In short, if you are going to deploy some infrastructure that are only for your k8s deployments, e.g. load balancers, IAM Roles for IRSA. Consider Crossplane. If you are going to deploy some shared infrastructure or it is not relevant to your k8s deployments, e.g. Network, EC2 bastions. Use Terraform.

## k8s infrastracture & application for production ready k8s
in an easy way

https://github.com/vfarcic/devops-toolkit-crossplane.git


## Crossplane - GitOps-based Infrastructure as Code through Kubernetes API
I want constrant sychronization between teh desired state & current state on resources as well. With teraform if someone deletes a machine or resource thsi change will be detected only when a push to git huppen through github piplenes that activate teraform resoure update & synch. On the other hand crossplane is embeded within k8s (crd) and therefore we can operate it through git opts tools and therofre keep the desired & current state much at any point through auto-such with repository

That practically means that we have ONE API to rule them all (applications, resources etc.), and this API is k8s API is gettting close to that.

* A gitOps kind of tool that will help me 
