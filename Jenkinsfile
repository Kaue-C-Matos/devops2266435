pipeline {
    agent any

    stages {
        stage('Executar testes') {
            steps {
                script {
                    sh'''
                        docker-compose up
                    '''
                }
            }
        }
    }
}
