 ### This project is very simple project. Just create EC2 Instances With UserData and SecurityGroup that allow permission SSH and HTTP.
 
 - [MyWebServerWithSecurityGroup.yaml](./Template/MyWebServerWithSecurityGroup.yaml)

 ### Create Stack
 ```bash
aws cloudformation create-stack --stack-name MyWebServerWithSecurityGroup --template-body file://MyWebServerWithSecurityGroup.yaml --parameters ParameterKey='KeyName',ParameterValue='SGkey'
```

 ### Update Stack
```bash
aws cloudformation update-stack --stack-name MyWebServerWithSecurityGroup --template-body file://MyWebServerWithSecurityGroup.yaml --parameters ParameterKey='KeyName',ParameterValue='SGkey'
```
### Delete Stack 
```bash
aws cloudformation delete-stack --stack-name MyWebServerWithSecurityGroup
```
