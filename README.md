# coresplain vs teraform
In short, if you are going to deploy some infrastructure that are only for your k8s deployments, e.g. load balancers, IAM Roles for IRSA. Consider Crossplane. If you are going to deploy some shared infrastructure or it is not relevant to your k8s deployments, e.g. Network, EC2 bastions. Use Terraform.
