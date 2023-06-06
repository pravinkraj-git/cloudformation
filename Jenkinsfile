pipeline{
    agent any
        stages {
            stage{'Clone Repo'}
                steps {
                    sh "export AWS_DEFAULT_REGION=eu-west-2"
                    sh "aws cloudformation create-stack --stack-name myteststack --template-body file://createinstance.yml --region 'eu-west-1'"
                }
        }
}