pipeline {
    agent {
        // Define agent details here
    }
    stages {
        stage('Example stage 1') {
            environment {
                BITBUCKET_COMMON_CREDS = credentials('jenkins-bitbucket-common-creds')
            }
            steps {
                echo "username $BITBUCKET_COMMON_CREDS_USR"
                echo "password $BITBUCKET_COMMON_CREDS_PSW"
            }
        }
        stage('Example stage 2') {
            steps {
                //
                echo "====++++second stage++++===="
            }
        }
    }
}