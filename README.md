# Parley Infrastructure
Cloudformation scripts for setting up infrastructure for parley

## Useful Commands

####1. Package
```shell script
aws cloudformation package --template-file master.yaml --s3-bucket infrastructure.parley.abstractmechanics.co.uk --output-template-file master-deploy.yaml
```

####2. Deploy
```shell script
aws cloudformation deploy --template-file master-deploy.yaml --stack-name parley --capability CAPABILITY_IAM
```

####3. Delete
```shell script
aws cloudformation delete-stack --stack-name parley
```
