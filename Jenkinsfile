pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Step 1: Checkout Git repository
                git branch: 'main', credentialsId: '1ae62d74-81ec-4b38-8d24-8faa7f93539c', url: 'https://github.com/mohamedgaber353/task_bonus.git'
            }
        }
        stage('Execute Commands') {
            steps {
                // Step 2: Execute a Windows batch command
                bat '''@ECHO OFF
                dir
                PAUSE'''
            }
        }
    }
}
