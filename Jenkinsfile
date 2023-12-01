pipeline {
    agent any

    stages {
        stage('Construir NodeGoat') {
            steps {
                script {
                    sh'''
                        npm install
                    '''
                }
            }
        }
        stage('Rodar Testes') {
            steps {
                script {
                    sh'''
                        npm install
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
