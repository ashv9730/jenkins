pipeline {
    agent any
    stages {
        stage('Example stage 1') {
            environment {
                BITBUCKET_COMMON_CREDS = credentials('jenkins-bitbucket-common-creds')
            }
            steps {
                echo "username and passwd"
                sh('$BITBUCKET_COMMON_CREDS_USR:$BITBUCKET_COMMON_CREDS_PSW')
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