pipeline{
    agent any
        stages {
            stage('clone repo'){
                steps {
                    sh "export AWS_DEFAULT_REGION=eu-west-2"
                    sh "aws cloudformation create-stack --stack-name myteststack --template-body file://creates3.json --region 'eu-west-2'"
            }
        }
    }
}