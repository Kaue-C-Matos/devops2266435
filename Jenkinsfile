pipeline{
    agent any
    tools{nodejs 'node'}
    stages{
        stage('Construir aplicação NodeGoat'){
            steps{
                sh '''
                    npm install
                '''
            }
        }
        stage('Rodar testes'){
            steps{
                sh '''
                    npm test
                '''
            }
        }
        stage('Construir projetos'){
            steps{
                sh '''
                    docker-compose build
                '''
            }
        }
        
    }
}
