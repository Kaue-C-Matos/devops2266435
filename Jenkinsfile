pipeline{
    agent any
    
    stages{
        stage('test') {
            steps{
                sh '''
                    sudo docker-compose build
                    senha123 -S
                '''
            }
        }
    }
}