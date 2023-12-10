pipeline {
    agent any
    options {
        skipStagesAfterUnstable()
    }
    stages {

        stage("Aclean workscape"){
            steps{
               cleanWs()
            }
            
        }

        stage('Build stage') {
            steps {
               echo " hello 1 build"
            }
        }
        stage('Test stage'){
            steps {
                echo "test"
            }
        }
        stage('Deploy  stage') {
            steps {
                echo "deploy hello"
            }
        }
    }
}