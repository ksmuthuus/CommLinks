# Setup Kubernetes cluster via kops

## Setup bootstrapper server (EC2)

## Update Env Vars

```sh
  export AWS_ACCESS_KEY_ID=$(aws configure get aws_access_key_id)
  export AWS_SECRET_ACCESS_KEY=$(aws configure get aws_secret_access_key)
  export KOPS_STATE_STORE=s3://csdemo-com-kops-state-store #S3 bucket already created
  export NAME=csdemo.k8s.local
```

## Create and validate Cluster

```sh
kops create cluster --zones us-east-1a,us-east-1b ${NAME}
ssh-keygen -b 2048 -t rsa -f ~/.ssh/id_rsa
kops create secret --name ${NAME} sshpublickey admin -i ~/.ssh/id_rsa.pub
```

## Manage Cluster Config

```sh
echo $EDITOR
export EDITOR=nano
echo $EDITOR
kops edit cluster ${NAME}
```

## Update(Deploy) Cluster

```sh
 kops update cluster --name ${NAME} --yes

```

## Validate/View cluster

```sh
kops validate cluster
kops get cluster --name ${NAME}
kops get ig --name ${NAME}
```
