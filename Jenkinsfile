pipeline {
    agent any

    stages {
        stage('Executar testes') {
            steps {
                script {
                    sh'''
                        docker system prune -a --volumes -f
                        docker compose up -d --no-color --wait
                        docker compose ps
                    '''
                }
            }
        }
    }
}
