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

        stage('Build') {
            steps {
               echo "build"
            }
        }
        stage('Test'){
            steps {
                echo "test"
            }
        }
        stage('Deploy') {
            steps {
                echo "deploy"
            }
        }
    }
}