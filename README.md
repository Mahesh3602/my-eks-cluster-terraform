## prerequiste launch EKS cluster  
  cd eks-cluser
  terrraform init  
  ## add or ensure tags to modules module.aws_vpc.module.aws_vpc.aws_subnet.public_subnets
  "Kubernetes.io/role/elb" = "1" && "Kubernetes.io/role/internal-elb" = "1"

  terraform plan and apply.


  aws eks update-kubeconfig --name terraform-eks-cluster