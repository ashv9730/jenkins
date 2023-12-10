pipeline{
    agent any
    environment {
        EXAMPLE_CREDS = credentials('jenkins-bitbucket-common-creds')
    }
    stages{
        stage("example"){
            steps{
                echo "========executing A========"
                sh('curl -u $EXAMPLE_CREDS_USR:$EXAMPLE_CREDS_PSW https://example.com/')
            }
           
        }
    }
   
}