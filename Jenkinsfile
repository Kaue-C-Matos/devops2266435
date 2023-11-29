pipeline {
    agent any
    
    stages {
        stage('Preparar ambiente') {
            steps {
                // Aqui você pode adicionar os comandos necessários para preparar o ambiente,
                // como clonar o repositório NodeGoat e instalar dependências.
                sh 'git clone https://github.com/OWASP/NodeGoat.git'
                dir('NodeGoat') {
                    sh 'npm install'
                }
            }
        }
        
        stage('Executar testes') {
            steps {
                // Execute os testes presentes na pasta 'test' do NodeGoat.
                dir('NodeGoat') {
                    sh 'npm test'
                }
            }
        }
    }
}