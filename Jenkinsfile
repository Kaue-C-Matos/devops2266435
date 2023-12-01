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
        stage('Construindo Docker') {
            steps {
                sh '''
                    docker build .
                '''
            }
        }
        stage('Compose Docker') {
            steps {
                sh '''
                    docker compose up
                '''
            }
        }
    }
}
