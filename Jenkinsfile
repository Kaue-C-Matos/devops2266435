pipeline{
    agent any
    
    stages{
        stage('test') {
            steps{
                sh '''
                    sudo docker-compose up
                    -S senha123
                '''
            }
        }
    }
}