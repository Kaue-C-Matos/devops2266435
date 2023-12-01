pipeline {
    agent any

    stages {
        stage('Construir NodeGoat') {
            steps {
                script {
                    sh'''

                        npm --version
                    '''
                }
            }
        }
        stage('Rodar Testes') {
            steps {
                script {
                    sh'''
                        npm teste
                    '''
                }
            }
        }
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
