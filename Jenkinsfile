pipeline{
    agent{
        label "node"
    }

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