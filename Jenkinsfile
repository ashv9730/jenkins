pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                echo 'Cloning the code'
            }
        }
        stage('Build') {
            steps {
                echo 'This is Build Stage'
            }
        }
        stage('Push to Docker hub') {
            steps {
                echo 'This is Test stage'
            }
        }
        stage('Deployement') {
            steps {
                echo 'Deploying container'
            }
        }
    }
}