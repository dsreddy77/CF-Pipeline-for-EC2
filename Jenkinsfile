def INSTANCE_IP
pipeline {
  agent any
   stages {
	stage('Clone Repo') {
	 steps {
	sh "export AWS_DEFAULT_REGION=us-east-1"
	sh "aws cloudformation create-stack --stack-name teststack --template-body file://ec2.yaml --parameters ParameterKey=KeyName,ParameterValue=SudarsanaPemFile ParameterKey=InstanceType,ParameterValue=t2.micro --region 'us-east-1'"			
		}
	}
          }
	}

