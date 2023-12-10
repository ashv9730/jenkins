pipeline{
    agent any
    environment {
        AWS_ACCESS_KEY_ID     = credentials('jenkins-aws-secret-key-id')
        AWS_SECRET_ACCESS_KEY = credentials('jenkins-aws-secret-access-key')
    }
    stages{
        stage("Loging to aws"){
            steps{
                echo 'printing aws Access key'
                echo "Access Key: ${MY_SECRET_CREDS_USR}"
            }
           
        }
    }
}