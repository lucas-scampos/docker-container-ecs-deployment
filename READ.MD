### creating stack in AWS CloudFormation

- aws cloudformation create-stack --stack-name example-deployment --template-body file://./ecs.yaml --capabilities CAPABILITY_NAMED_IAM --parameters ParameterKey=Subnet1ID,ParameterValue=<subnet-1> ParameterKey=Subnet2ID,ParameterValue=<subnet-2> ParameterKey=VPCID,ParameterValue=<vpc-id>

### updating stack 

- aws cloudformation update-stack --stack-name example-deployment --template-body file://./ecs.yaml --capabilities CAPABILITY_NAMED_IAM --parameters ParameterKey=Subnet1ID,ParameterValue=<subnet-1> ParameterKey=Subnet2ID,ParameterValue=<subnet-2> ParameterKey=VPCID,ParameterValue=<vpc-id>

### cleaning up

- aws cloudformation delete-stack --stack-name example-deployment
