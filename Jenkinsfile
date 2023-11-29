pipeline {
    agent {
        docker {
            image 'node:latest' // Use a imagem Node.js como base
            args '-u root' // Execute como usuário root para permissões
        }
    }
    
    stages {
        stage('Executar testes') {
            steps {
                sh 'signIn'
            }
        }
    }
}