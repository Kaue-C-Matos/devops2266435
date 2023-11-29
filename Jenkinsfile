pipeline {
    agent any

    stages {
        stage('Executar testes') {
            steps {
                script {
                    docker-compose up
                }
            }
        }
    }
}
