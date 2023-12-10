pipeline {
    agent any
    // options {
    //     skipStagesAfterUnstable()
    // }
    stages {

        stage("Aclean workscape"){
            steps{
               cleanWs()
            }
            
        }

        stage('Build') {
            steps {
                sh 'make'
            }
        }
        stage('Test'){
            steps {
                sh 'make check'
                junit 'reports/**/*.xml'
            }
        }
        stage('Deploy') {
            steps {
                sh 'make publish'
            }
        }
    }
}