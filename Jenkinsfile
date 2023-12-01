pipeline{
    agent any
    tools{nodejs 'node'}
    stages{
        stage('nmp --version'){
            steps{
                sh '''
                    npm --version
                '''
            }
        }
    }
}
