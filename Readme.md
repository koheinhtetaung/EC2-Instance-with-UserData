 # This project is EC2 Instances With UserData and SecurityGroup that allow permission SSH and HTTP.
 #Create Stack
 ```bash
aws cloudformation create-stack --stack-name MyWebServerWithSecurityGroup --template-body file://MyWebServerWithSecurityGroup.yaml --parameters ParameterKey='KeyName',ParameterValue='SGkey'
```

 #Update Stack
```bash
aws cloudformation update-stack --stack-name MyWebServerWithSecurityGroup --template-body file://MyWebServerWithSecurityGroup.yaml --parameters ParameterKey='KeyName',ParameterValue='SGkey'
```
#Delete Stack 
```bash
aws cloudformation delete-stack --stack-name MyWebServerWithSecurityGroup
```
