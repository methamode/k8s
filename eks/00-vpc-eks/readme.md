# Quickest way to Install EKS

This will provision a VPC and EKS.
## Pre requisite
Install the following tools:

1. [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/#install-kubectl-on-linux)
2. [aws-cli](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)

## How to verify if EKS has been provision successfully

```
1. Get Access token in the AWS account where you provision the EKS.
2. Get your kubeconfig to access your EKS Cluster 
 # aws eks update-kubeconfig --region ap-southeast-1 --name demo-eks
3. Run nginx pod to check if no issue in the pulling-in image(s)
 # kubectl run pod --image=nginx
4. Verify if your pods are running.
 # kubectl get pod -A

```

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)