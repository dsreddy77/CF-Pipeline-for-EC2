pipeline {
  agent any
   stages {
	stage('Clone Repo') {
	 steps {
	sh "export AWS_DEFAULT_REGION=us-east-1"
	sh "aws cloudformation create-stack --stack-name teststack --template-body file://CFforEC2.json  --region 'us-east-1'"
					}
				}
		}
	}

