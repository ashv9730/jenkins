pipeline{
    agent any

    environment {
        CC = 'CLang'
    }

    stages{
        stage("Example"){
            environment { 
                DEBUG_FLAGS = '-g'
            }
            steps{
                echo "printenv"
            }
            
        }
    }
    
}