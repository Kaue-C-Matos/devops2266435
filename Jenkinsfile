pipeline {
    agent any

    stages {
        stage('Checar versão do docker') {
            steps {
                script {
                    sh'''
                        docker-compose --version
                    '''
                }
            }
        }
        stage('Buildar docker') {
            steps {
                script {
                    sh'''
                        docker-compose build
                        docker-compose up
                    '''
                }
            }
        }
    }
}
