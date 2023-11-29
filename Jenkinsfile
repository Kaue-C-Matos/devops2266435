pipeline {
    agent any

    stages {
        stage('Executar testes') {
            steps {
                script {
                    sh 'sudo docker run node:latest npm test'
                }
            }
        }
    }
}
