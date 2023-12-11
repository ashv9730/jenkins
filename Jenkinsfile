pipeline {
    agent any
    environment {
      DOCKER_CRED = credentials('jenkins-bitbucket-common-creds')
    }
    stages {
        stage('Clone Code') {
            steps {
                echo 'Cloning the code'
                git url:"https://github.com/ashv9730/dashboard-python-nodejs.git", branch:"master"
            }
        }
        stage('Build') {
            steps {
                echo 'This is Build Stage'
                sh "docker build -t notes-app ."
            }
        }
        stage('Push to Docker hub') {
            steps {
                echo 'This is Test stage'
                sh "docker tag notes-app ${env.DOCKER_CRED_USR}/notes-app:latest"
                sh "docker login -u ${env.DOCKER_CRED_USR} -p ${env.DOCKER_CRED_PSW}" 
                sh "docker push ${env.DOCKER_CRED_USR}/notes-app:latest"
            }
        }
        stage('Deployement') {
            steps {
                echo 'Deploying container'
                sh "docker-compose down && docker-compose up -d"
            }
        }
    }
}