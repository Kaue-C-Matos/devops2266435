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
        stage('Rodat testes'){
            steps{
                sh '''
                    npm test
                '''
            }
        }
    }
}
