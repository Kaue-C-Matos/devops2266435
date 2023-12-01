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
        stage('Construindo projeto nos containers') {
            steps {
                sh '''
                    docker build .
                '''
            }
        }
        stage('Rodando projeto nos containers') {
            steps {
                sh '''
                    docker compose up
                '''
            }
        }
    }
}
