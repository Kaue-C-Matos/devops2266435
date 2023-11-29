pipeline{
    agent any
    
    environment {
        MY_PASSWORD = credentials('sudosenha')
    }

    stages{
        stage('test') {
            steps{
                script {
                    withCredentials([string(credentialsId: 'sudosenha', variable: 'MY_PASSWORD')]) {
                        sh "echo $MY_PASSWORD | sudo -S docker-compose  up" // Substitua o comando pelo que você deseja executar com sudo
                    }
                }
            }
        }
    }
}