pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
        stage('Cloning git') {
            steps {
                git 'https://github.com/gustavoapolinario/node-todo-frontend'
            }
        }
        stage('Install dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}
